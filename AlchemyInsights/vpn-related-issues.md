---
title: Problèmes liés au réseau privé virtuel
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505188"
---
# <a name="vpn-related-issues"></a>Problèmes liés au réseau privé virtuel

L’implémentation réussie de la connectivité VPN pour les clients de la gestion des périphériques mobiles dépend d’un profil déployé qui reflète correctement les exigences de l’infrastructure VPN. Pour connaître les paramètres appropriés pour les plateformes client que vous examinez, consultez : 

[Paramètres des appareils Windows 10 et Windows holographiques pour ajouter des connexions VPN à l’aide de Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Ajouter des paramètres VPN sur les appareils iOS et iPad dans Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Paramètres de l’appareil Android pour configurer le VPN dans Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Ajouter des paramètres VPN sur les appareils macOS dans Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Si votre profil VPN utilise l’authentification basée sur les certificats, assurez-vous que les profils de certificats racine et d’authentification de client liés au profil VPN sont correctement déployés.

**Problèmes courants**

**J’ai déployé un profil réseau privé virtuel sur un appareil. Intune indique qu’il a réussi, mais que l’appareil ne se connecte pas au réseau privé virtuel.**

L’état réussite indique que Intune a correctement déployé le profil configuré. Toutefois, il est possible que ces configurations ne correspondent pas à votre réseau ou d’autres exigences d'authentification. Consultez les journaux dans le service d’infrastructure et d’authentification (sur le serveur VPN et le serveur NPS/RADIUS) pour plus d’informations sur la tentative de connexion. Il se peut que vous deviez collaborer avec l’équipe de votre infrastructure réseau ou le fournisseur VPN tiers pour recueillir et consulter les journaux.

**Lorsque je configure un réseau privé virtuel (VPN) personnalisé pour iOS, la fonctionnalité VPN par application n’est pas mise à disposition.**

Le VPN par application pour les appareils iOS dans Intune est actuellement disponible pour une liste spécifique de fournisseurs et de partenaires, qui doivent également satisfaire les conditions préalables requises pour configurer un VPN par application. Pour plus d’informations, consultez [Configurer le réseau privé virtuel (VPN) par application pour les appareils iOS/iPad dans Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Pour plus d’informations sur tous les types de connexions VPN dans Intune, consultez [Créer des profils VPN pour se connecter aux serveurs VPN dans Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

** Le VPN à la demande d'iOS ne se déclenche pas lors de l'accès à un domaine configuré**

Pour tester les paramètres VPN automatiques, configurez les valeurs suivantes :

Je veux effectuer les opérations suivantes : **évaluer chaque tentative de connexion** 

Indiquez si vous voulez vous connecter : **se connecter si nécessaire**

Lorsque les utilisateurs accèdent à ces domaines : **cible** *nom de domaine*

Si la configuration ci-dessus échoue, ajoutez l’élément suivant :

Lorsque cette URL est inaccessible, forcez la connexion du VPN : **BADURL**