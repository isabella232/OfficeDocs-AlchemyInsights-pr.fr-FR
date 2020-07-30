---
title: Résolution des problèmes de déploiement des certificats d’authentification client
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509052"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Résolution des problèmes de déploiement des certificats d’authentification client

Les profils de certificats clients Intune NDES/SCEP et PKCS/PFX sont généralement utilisés conjointement avec d’autres types de profils tels que WiFi, VPN et e-mail pour permettre aux utilisateurs de s’authentifier auprès des ressources d’entreprise. Lorsque ces types de profils sont liés à un profil de certificat client dépendent du déploiement réussi de ce profil.

La configuration initiale de l’infrastructure et la configuration associée du profil de certificat client nécessitent souvent une résolution des problèmes. Pour consulter un guide détaillé de la configuration réussie du connecteur NDES et des instructions de dépannage pour isoler les problèmes liés au déploiement de certificats, voir : 

- [Configurer l’infrastructure pour la prise en charge de SCEP avec Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Vue d’ensemble de la résolution des problèmes de profils de certificats SCEP avec Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Utilisez les scripts PowerShell référencés pour vérifier votre configuration. Pour plus d’informations, voir [scripts de vérification du connecteur de certificats Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Autres problèmes courants**

**Lorsque j’essaie d’installer le connecteur de certificats Intune sur le serveur NDES Connector, je reçois le message «le mot de passe de la demande de certificat ne peut pas être vérifié. Elle a peut-être déjà été utilisée. Obtenez un nouveau mot de passe à envoyer avec cette demande.»**  

Ce message signifie que vous devez exécuter l’installation du connecteur de certificats en tant qu’administrateur.

Dans certains environnements, les serveurs sur lesquels le certificat Intune s’exécute doivent utiliser un serveur proxy pour se connecter à Intune. par conséquent, le connecteur de certificat doit utiliser un proxy. Dans certains cas, le connecteur NDES ignore les paramètres de proxy configurés et peut être nécessaire pour configurer les paramètres de proxy pendant l’exécution dans le contexte de sécurité LocalSystem. 
 
La solution consiste à exécuter Internet Explorer en tant que système et à configurer un proxy dans Internet Explorer. Après un redémarrage du service Intune Connector, le connecteur NDES se connecte à Intune.

**Les appareils utilisateur ne reçoivent plus les certificats SCEP de NDES.**

Il est possible que le certificat d’authentification de client émis pour le serveur NDES, et spécifié lors de l’installation du connecteur NDES, ait expiré ou est manquant. Pour résoudre : 
 
1. Désinstallez le connecteur NDES.  
2. Utilisez ces détails pour demander un nouveau certificat d’authentification de client ou de serveur : 
 
    - Nom du sujet : CN = FQDN externe  
    - Nom de l’autre objet (obligatoire) : DNS = nom de domaine complet (FQDN) externe, DNS = nom de domaine complet interne 
 
3. Réinstallez le connecteur NDES avec le nouveau certificat.