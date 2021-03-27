---
title: Obtenir la liste des applications d’entreprise
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379852"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="391ef-102">Obtenir la liste des applications d’entreprise</span><span class="sxs-lookup"><span data-stu-id="391ef-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="391ef-103">Pour obtenir une liste **d’applications** d’entreprise (toutes les applications ou filtrées par nom d’affichage, ID, URL d’identificateur, etc.) via la commande Powershell, voir [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="391ef-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="391ef-104">Pour obtenir la liste des objets principaux de service (tous les objets ou filtrés par ID) via la commande Powershell, voir [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="391ef-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="391ef-105">Si vous souhaitez obtenir la liste des applications **saml configurées, les scripts PowerShell suivants** peuvent vous aider :</span><span class="sxs-lookup"><span data-stu-id="391ef-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="391ef-106">Chaque application, qu’il s’agit d’une application OAuth ou d’une application SAML (applications galerie et non galerie) aurait deux objets créés dans AAD lors de leur inscription.</span><span class="sxs-lookup"><span data-stu-id="391ef-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="391ef-107">L’un est appelé objet Application et l’autre est l’objet Principal de service.</span><span class="sxs-lookup"><span data-stu-id="391ef-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="391ef-108">Lorsque vous videz les propriétés d’un objet principal de service à l’aide de PowerShell, vous constatez que chaque application possède un certain nombre de balises associées comme :</span><span class="sxs-lookup"><span data-stu-id="391ef-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="391ef-109">Les applications OAuth auraient une balise appelée **« WindowsAzureActiveDirectoryIntegratedApp**»</span><span class="sxs-lookup"><span data-stu-id="391ef-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="391ef-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**»</span><span class="sxs-lookup"><span data-stu-id="391ef-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="391ef-111">Les applications SAML autres que gallery auraient une balise appelée **« WindowsAzureActiveDirectoryCustomSingleSignOnApplication**»</span><span class="sxs-lookup"><span data-stu-id="391ef-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="391ef-112">Par conséquent, vous pouvez utiliser ces balises et découvrir le type d’application qu’il s’agit.</span><span class="sxs-lookup"><span data-stu-id="391ef-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="391ef-113">La balise **« WindowsAzureActiveDirectoryIntegratedApp**» est commune à tous les types d’applications.</span><span class="sxs-lookup"><span data-stu-id="391ef-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="391ef-114">Vous pouvez utiliser l’extrait de code suivant pour ré lister toutes les applications SAML (galerie et non galerie) :</span><span class="sxs-lookup"><span data-stu-id="391ef-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="391ef-115">Pour plus d’informations, voir Identifier les applications [saml dans Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="391ef-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="391ef-116">**Rechercher et lister uniquement les applications Web**: utilisez la commande ci-dessous pour obtenir toutes les applications Azure AD avec le type d’application « Application Web/API »</span><span class="sxs-lookup"><span data-stu-id="391ef-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="391ef-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="391ef-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="391ef-118">**Recherchez et listez les applications natives uniquement**: exécutez la commande suivante pour obtenir toutes les applications clientes natives (ordinateur de bureau/appareil mobile).</span><span class="sxs-lookup"><span data-stu-id="391ef-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="391ef-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="391ef-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="391ef-120">**Exporter tous les détails** de l’application Azure AD enregistrée vers CSV : la commande ci-dessous exporte toutes les applications Azure AD avec les détails requis dans le fichier csv :</span><span class="sxs-lookup"><span data-stu-id="391ef-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="391ef-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="391ef-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="391ef-122">Export-Csv « C:\AzureADApps.csv » -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="391ef-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="391ef-123">**Besoin d’exporter une liste d’applications Azure inutilisées** – Rapport d’audit</span><span class="sxs-lookup"><span data-stu-id="391ef-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="391ef-124">Azure AD peut afficher les journaux d’application pendant 30 jours uniquement à condition que vous donnent une licence Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="391ef-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="391ef-125">Vous avez deux options pour conserver les données pendant plus de 30 jours.</span><span class="sxs-lookup"><span data-stu-id="391ef-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="391ef-126">Vous pouvez utiliser les API de rapports [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) pour récupérer les données par programme et les stocker dans une base de données.</span><span class="sxs-lookup"><span data-stu-id="391ef-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="391ef-127">Vous pouvez également intégrer des journaux d’audit dans un système SIEM tiers.</span><span class="sxs-lookup"><span data-stu-id="391ef-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="391ef-128">Vous pouvez également télécharger la liste des applications pour toutes les applications et les applications propriétaire sous Azure Active Directory>App Registrations>Télécharger>Toutes les applications/applications propriétés.</span><span class="sxs-lookup"><span data-stu-id="391ef-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="391ef-129">Pour obtenir la liste des applications via MS Graph, voir Applications de liste [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) et type de ressource d’application [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="391ef-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
