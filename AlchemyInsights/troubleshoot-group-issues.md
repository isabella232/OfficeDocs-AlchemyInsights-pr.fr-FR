---
title: Résoudre les problèmes de groupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716107"
---
# <a name="troubleshoot-group-issues"></a>Résoudre les problèmes de groupe

**J’ai besoin d’attribuer à un groupe à un rôle Azure AD**

Pour attribuer un rôle Azure Active Directory (AD) à un groupe Azure Active Directory, effectuez les étapes suivantes :

1. Créer un groupe : Pour créer un groupe :

    a. Connectez-vous au centre d’administration Azure AD avec des autorisations d’administrateur de rôle privilégié ou d’administrateur général. 
    b. Sélectionnez Azure Active Directory > Groupes > Tous les groupes > Nouveau groupe. 
    c. Créer le groupe.

2. Attribuez le rôle au groupe lors de la création du groupe ou après la création du groupe.

    a. Pour attribuer un rôle au groupe au moment de la création du groupe, basculez sur le bouton bascule Des rôles Azure AD peuvent être attribués au groupe, puis créer le groupe.
    b. Pour attribuer un rôle au groupe après sa création, accédez à l’onglet Rôles attribués du nouveau groupe, puis attribuez le rôle au groupe.

**J’ai besoin de gérer l’adhésion à un groupe affecté à un rôle Azure AD**

1. Pour empêcher l’élévation des privilèges, par défaut, seuls l’administrateur de rôle privilégié et l’administrateur général peuvent modifier l’adhésion d’un groupe affecté à un rôle. Toutefois, ils peuvent choisir d’affecter un propriétaire à un tel groupe et déléguer cette tâche. Pour plus d’informations, consultez [Utiliser des groupes cloud pour gérer les attributions de rôles dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Pour les questions courantes et conseils de dépannage pour l’attribution de rôles à des groupes dans Azure AD, consultez [Résolution des problèmes des rôles affectés aux groupes cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Groupes dynamiques**

1. Si vous ne trouvez pas les attributs utilisateur intégrés, assurez-vous que l'attribut figure dans la liste des propriétés prises en charge.
2. Si vous recherchez des attributs intégrés à l’appareil, assurez-vous que l’attribut figure dans la liste des attributs de l’appareil. 
3. Outre les attributs intégrés à l’utilisateur et à l’appareil, vous pouvez également utiliser [Attributs d'extension](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Après avoir synchronisé les attributs d'extension à partir de Windows Server AD sur site ou d'une application SaaS connectée, les attributs doivent être visibles dans la liste déroulante du générateur de règles. Le nom de l'attribut personnalisé peut être trouvé dans le répertoire en interrogeant l'attribut d'un utilisateur à l'aide de PowerShell et en recherchant le nom de l'attribut. Ils peuvent également être utilisés lors de la construction de règles dans la syntaxe des règles.
4. Assurez-vous que votre client dispose de la licence appropriée. Les groupes dynamiques requièrent au client une licence Azure AD P1 Premium. Vous pouvez consulter la liste des plans de licence Azure AD [ici](https://azure.microsoft.com/pricing/details/active-directory/). Vous pouvez accéder aux plans de gestion des licences Enterprise Mobility + Security [ici](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Assurez-vous que le rôle de l'utilisateur qui crée le groupe dynamique est un administrateur général, un administrateur intune, un administrateur de groupe ou un administrateur utilisateur.
6. Veuillez laisser le temps au groupe de se remplir. Selon la taille de votre client, le groupe peut prendre jusqu'à 24 heures pour se remplir pour la première fois ou après une modification des règles.
7. Pour plus d’informations, consultez [Créer règles basées sur les attributs pour l’appartenance au groupe dynamique](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**J’ai besoin de supprimer un groupe**

1. Les groupes peuvent être supprimés de l’annuaire à l’aide de la cmdlet Remove-AzureADGroup du module Azure AD Powershell.
2. Avant d’essayer de supprimer un groupe synchronisé dans Azure AD, assurez-vous que vous avez supprimé toutes les licences attribuées pour éviter les erreurs.
3. Pour plus d’informations sur la suppression de groupes, consultez [Suppression d’un groupe avec une licence attribuée](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**J’ai besoin de restaurer un groupe supprimé**

1. Si un groupe Office 365 est supprimé, il ne peut être restauré que 30 jours avant la suppression définitive. Une fois supprimé de manière définitive, le groupe ne peut plus être restauré. En savoir plus sur la restauration des groupes [ici](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Cette fonctionnalité n’est pas prise en charge pour les groupes de sécurité et les groupes de distribution.
3. Assurez-vous que vous êtes autorisé à restaurer un groupe Office 365. Les administrateurs généraux, les administrateurs de groupes, les administrateurs de comptes d'utilisateurs, les administrateurs de services intune, le support partenaire de niveau 1 ou 2 et le propriétaire du groupe peuvent être en mesure de restaurer un groupe.
4. Lorsqu’un groupe dynamique est supprimé et restauré, il est considéré comme un nouveau groupe et rempli en fonction de la règle. Ce processus peut prendre jusqu’à 24 heures.
5. Pour plus d’informations sur la restauration d’un groupe supprimé, consultez [Restaurer un groupe Office 365 supprimé dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Configuration d’une stratégie d’expiration de groupe**

1. Cette fonctionnalité est uniquement prise en charge pour les groupes Office 365, et non pour les groupes de sécurité et les groupes de distribution.
2. La configuration et l’utilisation de la stratégie d’expiration pour les groupes Office 365 nécessitent une licence Azure AD Premium.
3. Actuellement, une seule stratégie d’expiration peut être configurée pour les groupes Office 365 sur un client.
4. Seuls les administrateurs généraux, les administrateurs de groupe, les administrateurs utilisateurs et le propriétaire du groupe peuvent renouveler un groupe.
5. Si un groupe Office 365 a expiré, il est supprimé et ne peut être restauré que 30 jours avant la suppression définitive. Une fois supprimé de manière définitive, le groupe ne peut plus être restauré. En savoir plus sur la restauration des groupes [ici](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Renouvellement automatique basé sur l’activité**

Les activités des utilisateurs dans SharePoint, Outlook et Teams peuvent déclencher le renouvellement automatique de groupe. Les activités sont cochées 35 jours avant l’expiration d’un groupe. En cas d’activité pendant le cycle de vie du groupe, le groupe est renouvelé automatiquement et la notification par courrier électronique n’est pas envoyée aux propriétaires du groupe.

**Calendrier des notifications pour les groupes expirés**

1. Les notifications par courrier électronique sont envoyées aux propriétaires du groupe Office 365 30 jours, 15 jours et 1 jour avant l’expiration du groupe.
2. Lorsque vous définissez la date d’expiration pour la première fois, tous les groupes qui sont supérieurs à l’intervalle d’expiration sont fixés à 35 jours avant la date d’expiration.
3. La date d’expiration du groupe est calculée en fonction de la date de renouvellement du groupe, et non en fonction de la date de mise à jour de la stratégie. Si la stratégie d’expiration est mise à jour, la date d’expiration ne change pas.
4. Pour plus d’informations, consultez [Stratégie d'expiration des groupes et courriels de renouvellement](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) et [Restaurer un groupe Office 365 supprimé dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Autorisation de création d’un groupe**

Assurez-vous que vous êtes autorisé à créer un groupe. Les administrateurs généraux peuvent désactiver la création de groupes dans le Portail Azure ou le panneau d’accès. Il se peut que vous ayez besoin d'un administrateur pour créer le nouveau groupe pour vous, ou pour vous donner les autorisations appropriées.

1. [Créer un groupe et ajouter des membres dans le Portail Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Créer des groupes dans Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Désactiver la création de groupes dans PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Gérer les personnes autorisées à créer des groupes dan Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Désactiver la notification d’accueil d’Office 365 via PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Rôles d’administration d’Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Gérer les autorisations de création de groupes**

1. Les administrateurs généraux peuvent gérer les autorisations de création de groupes de sécurité ou de groupes Office 365 créés dans le portail Azure ou dans le volet d’accès, en définissant les paramètres **Les utilisateurs peuvent créer des groupes de sécurité dans les portails Azure** ou **Les utilisateurs peuvent créer des groupes Office 365 dans les Portails Azure** dans **Tous les groupes > Général (Paramètres)**.
2. Vous pouvez également restreindre la création de groupes pour sélectionner un groupe d’utilisateurs si vous avez une licence Azure AD P1 Premium.

**Désactivation de la notification d’accueil pour les nouveaux membres d’un groupe Office 365**

La notification de bienvenue envoyée aux utilisateurs ajoutés à des groupes Office 365 peut être désactivée en définissant `UnifiedGroupWelcomeMessageEnabled` sur **Faux** dans PowerShell. En savoir plus sur ce paramètre [ici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













