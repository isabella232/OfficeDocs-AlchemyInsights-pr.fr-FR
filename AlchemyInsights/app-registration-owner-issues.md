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
# <a name="app-registration-owner-issues"></a><span data-ttu-id="52342-102">Problèmes du propriétaire de l’inscription de l’application</span><span class="sxs-lookup"><span data-stu-id="52342-102">App Registration Owner issues</span></span>

<span data-ttu-id="52342-103">Voici les méthodes disponibles pour ajouter des principaux en tant que propriétaires pour les inscriptions d’applications :</span><span class="sxs-lookup"><span data-stu-id="52342-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="52342-104">Utilisation du module Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="52342-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="52342-105">Référence : [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="52342-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="52342-106">Utilisation d’Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="52342-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="52342-107">Référence : [propriétaire de l’application az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="52342-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="52342-108">Utilisation de MS Graph -</span><span class="sxs-lookup"><span data-stu-id="52342-108">Using MS Graph -</span></span>

    <span data-ttu-id="52342-109">Référence : [Ajouter un propriétaire - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="52342-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="52342-110">Utilisation du portail Azure AD : accédez à [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Sélectionnez votre application > propriétaires > ajouter des propriétaires</span><span class="sxs-lookup"><span data-stu-id="52342-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="52342-111">**Vous ne pouvez pas afficher votre application dans le blade Inscriptions de l’application, même si vous êtes le propriétaire de cette application ?**</span><span class="sxs-lookup"><span data-stu-id="52342-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="52342-112">Le propriétaire d’une application n’est pas un rôle administratif.</span><span class="sxs-lookup"><span data-stu-id="52342-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="52342-113">Si le paramètre Restreindre l’accès au portail [d’administration Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) est activé, seul l’administrateur sera en mesure d’afficher les applications sur le portail d’inscription des applications.</span><span class="sxs-lookup"><span data-stu-id="52342-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="52342-114">Pour qu’un propriétaire puisse afficher les applications, désactivez ce paramètre (définissez ce paramètre sur NON) ou attribuez un rôle d’administrateur au propriétaire uniquement pour l’application spécifique.</span><span class="sxs-lookup"><span data-stu-id="52342-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="52342-115">Toutefois, pour cela, vous aurez besoin d’une licence Azure AD Premium P2 et activez [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span><span class="sxs-lookup"><span data-stu-id="52342-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
