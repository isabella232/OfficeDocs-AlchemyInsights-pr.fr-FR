---
title: Problèmes du propriétaire de l’inscription de l’application
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
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123112"
---
# <a name="app-registration-owner-issues"></a>Problèmes du propriétaire de l’inscription de l’application

Voici les méthodes disponibles pour ajouter des principaux en tant que propriétaires pour les inscriptions d’applications :

- Utilisation du module Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Référence : [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Utilisation d’Azure CLI - `az ad app owner add`

    Référence : [propriétaire de l’application az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Utilisation de MS Graph -

    Référence : [Ajouter un propriétaire - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Utilisation du portail Azure AD : accédez à [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Sélectionnez votre application > propriétaires > ajouter des propriétaires

**Vous ne pouvez pas afficher votre application dans le blade Inscriptions de l’application, même si vous êtes le propriétaire de cette application ?**

Le propriétaire d’une application n’est pas un rôle administratif. Si le paramètre Restreindre l’accès au portail [d’administration Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) est activé, seul l’administrateur sera en mesure d’afficher les applications sur le portail d’inscription des applications. Pour qu’un propriétaire puisse afficher les applications, désactivez ce paramètre (définissez ce paramètre sur NON) ou attribuez un rôle d’administrateur au propriétaire uniquement pour l’application spécifique. Toutefois, pour cela, vous aurez besoin d’une licence Azure AD Premium P2 et activez [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).
