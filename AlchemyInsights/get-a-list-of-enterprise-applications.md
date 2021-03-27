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
# <a name="get-a-list-of-enterprise-applications"></a>Obtenir la liste des applications d’entreprise

1. Pour obtenir une liste **d’applications** d’entreprise (toutes les applications ou filtrées par nom d’affichage, ID, URL d’identificateur, etc.) via la commande Powershell, voir [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Pour obtenir la liste des objets principaux de service (tous les objets ou filtrés par ID) via la commande Powershell, voir [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Si vous souhaitez obtenir la liste des applications **saml configurées, les scripts PowerShell suivants** peuvent vous aider :

    Chaque application, qu’il s’agit d’une application OAuth ou d’une application SAML (applications galerie et non galerie) aurait deux objets créés dans AAD lors de leur inscription. L’un est appelé objet Application et l’autre est l’objet Principal de service. Lorsque vous videz les propriétés d’un objet principal de service à l’aide de PowerShell, vous constatez que chaque application possède un certain nombre de balises associées comme :

    - Les applications OAuth auraient une balise appelée **« WindowsAzureActiveDirectoryIntegratedApp**»
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**»
    - Les applications SAML autres que gallery auraient une balise appelée **« WindowsAzureActiveDirectoryCustomSingleSignOnApplication**»

    Par conséquent, vous pouvez utiliser ces balises et découvrir le type d’application qu’il s’agit. La balise **« WindowsAzureActiveDirectoryIntegratedApp**» est commune à tous les types d’applications. Vous pouvez utiliser l’extrait de code suivant pour ré lister toutes les applications SAML (galerie et non galerie) :

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Pour plus d’informations, voir Identifier les applications [saml dans Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Rechercher et lister uniquement les applications Web**: utilisez la commande ci-dessous pour obtenir toutes les applications Azure AD avec le type d’application « Application Web/API »

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Recherchez et listez les applications natives uniquement**: exécutez la commande suivante pour obtenir toutes les applications clientes natives (ordinateur de bureau/appareil mobile).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Exporter tous les détails** de l’application Azure AD enregistrée vers CSV : la commande ci-dessous exporte toutes les applications Azure AD avec les détails requis dans le fichier csv :

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv « C:\AzureADApps.csv » -NoTypeInformation -Encoding UTF8

7. **Besoin d’exporter une liste d’applications Azure inutilisées** – Rapport d’audit

    Azure AD peut afficher les journaux d’application pendant 30 jours uniquement à condition que vous donnent une licence Azure AD Premium.
    Vous avez deux options pour conserver les données pendant plus de 30 jours. Vous pouvez utiliser les API de rapports [Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) pour récupérer les données par programme et les stocker dans une base de données. Vous pouvez également intégrer des journaux d’audit dans un système SIEM tiers.

    Vous pouvez également télécharger la liste des applications pour toutes les applications et les applications propriétaire sous Azure Active Directory>App Registrations>Télécharger>Toutes les applications/applications propriétés.

    Pour obtenir la liste des applications via MS Graph, voir Applications de liste [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) et type de ressource d’application [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
