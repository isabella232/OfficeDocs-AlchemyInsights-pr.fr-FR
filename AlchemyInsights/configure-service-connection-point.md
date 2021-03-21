---
title: Configurer le point de connexion de service (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897733"
---
# <a name="configure-service-connection-point-scp"></a>Configurer le point de connexion de service (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Raison** : impossible de lire l’objet SCP et d’obtenir les informations du client Azure AD
- **Résolution** : reportez-vous à la section [Configurer un point de connexion au service](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Plan d’action**

- Vérifiez si l’appareil a reçu l’objet de stratégie de groupe pour la validation contrôlée.
- Assurez-vous que l’objet de stratégie de groupe a créé les clés de Registre.
- Assurez-vous que vous avez deux clés créées avec votre ID d’annuaire et votre domaine onmicrosoft.

**Configurer le paramètre de Registre côté client pour le protocole SCP**

Utilisez l’exemple suivant pour créer un objet de stratégie de groupe afin de déployer un paramètre de Registre qui configure une entrée SCP dans le Registre de vos appareils.

1. Ouvrez une console de gestion des stratégies de groupe et créez un nouveau groupe de stratégies de groupe dans votre domaine.
     - Donnez un nom à votre objet de stratégie de groupe nouvellement créée (par exemple, ClientSideSCP)

2. Modifiez l'objet de stratégie de groupe et recherchez le chemin d'accès suivant : **Configuration de l’ordinateur > Préférences > Paramètres Windows > Registre**.

3. Cliquez avec le bouton droit sur **Registre**, sélectionnez **Nouveau > Élément de Registre**.

4. Dans l'onglet **Général**, configurez les éléments suivants :
  
- **Action** : Mise à jour
    
- **Hive** : HKEY_LOCAL_MACHINE
    
- **Chemin d’accès** : SOFTWARE\Microsoft\Windows\CurrentVersion\C PATH\AAD
    
- **Nom de la valeur** : TenantId
    
- **Type de valeur** : REG_SZ
    
- **Données de valeur** : GUID ou ID d’annuaire de votre instance Azure AD (cette valeur est dans **Portail Azure > Azure Active Directory > Propriétés > ID d’annuaire**)
 
- Cliquez sur **OK**.
 
5. Cliquez avec le bouton droit sur **Registre**, sélectionnez **Nouveau > Élément de Registre**.

6. Dans l'onglet **Général**, configurez les éléments suivants :
  
- **Action** : Mise à jour
    
- **Hive** : HKEY_LOCAL_MACHINE
    
- **Chemin d’accès** : SOFTWARE\Microsoft\Windows\CurrentVersion\C PATH\AAD
    
- **Nom de la valeur** : TenantName
    
- **Type de valeur** : REG_SZ
    
- **Données de valeur** : votre nom de domaine vérifié si vous utilisez un environnement fédéré tel qu’AD FS. Votre nom de domaine vérifié ou votre nom de domaine onmicrosoft.com (par exemple, contoso.onmicrosoft.com si vous utilisez un environnement géré).

- Cliquez sur **OK**.

7. Fermez l’éditeur du nouvel éditeur.

8. Liez l’objet de stratégie de groupe nouvellement créé à l'OU souhaitée contenant les ordinateurs joints au domaine qui appartiennent à votre population de déploiement contrôlé.

Pour plus d’informations, consultez [Validation contrôlée de la jonction Azure AD Hybride - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) et [Résolution des problèmes des appareils joints Azure Active Directory hybrides | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









