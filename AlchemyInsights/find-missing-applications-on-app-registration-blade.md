---
title: Rechercher les applications manquantes dans le blade d’inscription de l’application
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123090"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Rechercher les applications manquantes dans le blade d’inscription de l’application

1. Impossible de trouver des applications sur le portail d’inscription des applications.

    Si une application est une application multi-client et qu’elle a été inscrite dans un autre client, elle ne s’affichera pas sous le blade d’inscription de l’application. Toutefois, vous pouvez le trouver sous le lame Applications d’entreprise une fois qu’il a été accédé (après avoir reçu son consentement) et que le principal de service a été créé dans votre client. Pour plus d’informations, voir Applications & principaux de [service dans Azure AD - plateforme d’identité Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Impossible d’afficher les applications dans le panneau Inscription de l’application, même si vous êtes un administrateur.

    Assurez-vous que vous êtes dans le bon répertoire sur le portail Azure.
3. Mon application n’est pas répertoriée sous le lame Applications d’entreprise, mais elle s’affiche lorsque j’interroge la commande PowerShell.

    Parfois, après avoir supprimé l’application du portail Azure, elle n’est pas présente dans le portail, mais elle n’a peut-être pas été supprimée complètement. Pour plus d’informations, reportez-vous aux rubriques suivantes :
    - Vous pouvez récupérer la liste des applications supprimées précédemment et voir si l’application apparaît dans la liste à l’aide de la commande Powershell : **Get-AzureADDeletedApplication**. Pour plus d’informations, [voir Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Si vous souhaitez supprimer complètement l’application, vous pouvez essayer ce qui suit dans PowerShell : **Remove-AzureADApplication -ObjectId**. Pour plus d’informations, [voir Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Vous pouvez également essayer de restaurer l’application supprimée à l’aide de la commande Powershell suivante : **Restaurer AzureADDeletedApplication -ObjectId**. Pour plus d’informations, [voir Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Vous ne trouvez pas la liste de toutes les applications d’entreprise préinstallées dans mon nouveau client Azure.

    Il n’existe aucune application d’entreprise préinstallée dans Azure AD par défaut. Vous devez l’ajouter manuellement à partir de l’option « Nouvelle application » en la parcourant à partir de la galerie Azure AD ou en y ajouter une autre. Pour plus d’informations, voir Démarrage rapide : ajouter une application à votre client [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Si vous êtes un administrateur général, vous pouvez facilement accéder à vos applications à l’aide de [l’application Microsoft 365 Lanceur](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Impossible de trouver mes applications à partir du portail Mes applications.

    Assurez-vous que les applications ne sont pas masquées dans la page de la collection My Apps. Pour en savoir plus, consultez [Collections (prévisualisation)](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)dans le portail Mes applications - Azure AD .
6. Pour démarrer des applications à partir du portail Mes applications, voir Localiser & utiliser des applications sur le portail Mes applications [- Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. L’application Office 365 Mover ne s’affiche pas sur le panneau Applications d’entreprise après l’installation.

    L’application « Office 365 Mover » est une application à plusieurs entreprises qui n’a pas besoin d’être ajoutée à AAD à l’aide de la section Applications galerie sous Enregistrement des applications d’entreprise. Pour accéder à l’application Office 365 Mover, connectez-vous simplement à l’application et demandez le consentement de l’utilisateur pour les autorisations. Une fois que l’utilisateur a donné son consentement, cette application est automatiquement ajoutée au client avec l’ID de messagerie que vous avez connecté.

    Une fois l’application entrée, vous devriez être en mesure de trouver l’entrée de cette application sous le lame Applications d’entreprise dans AAD. Vous devez rechercher cette application en tapant le nom complet, c’est-à-dire « Office 365 Mover » ou simplement « office » et il doit lister l’application. Pour plus d’informations, voir Office 365 Mover indique qu’il est déjà installé, mais qu’il n’est pas répertorié dans la galerie [d’applications d’entreprise.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. Démarrage rapide : afficher la liste des applications qui utilisent votre client [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) pour la gestion des identités vous montre comment afficher les applications, également appelées applications, qui sont déjà définies pour utiliser votre client Azure AD en tant que fournisseur d’identité (IdP).
9. [Résoudre les problèmes courants liés](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) à l’ajout ou à la suppression d’une application dans Azure Active Directory vous permet de comprendre les problèmes courants auxquels les utilisateurs sont confrontés lors de l’affichage d’applications dans Azure Active Directory.
