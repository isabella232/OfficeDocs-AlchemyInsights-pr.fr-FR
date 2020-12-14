---
title: Aucun résultat renvoyé lors de la recherche/exportation de contenu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666643"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="bc1d8-102">Aucun résultat renvoyé lors de la recherche/exportation de contenu</span><span class="sxs-lookup"><span data-stu-id="bc1d8-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="bc1d8-103">Si vous rencontrez des problèmes avec les scénarios eDiscovery suivants :</span><span class="sxs-lookup"><span data-stu-id="bc1d8-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="bc1d8-104">Recherche/exportation de contenu ne renvoie aucune donnée ni aucune donnée inattendue</span><span class="sxs-lookup"><span data-stu-id="bc1d8-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="bc1d8-105">échec de la recherche eDiscovery ou de l’exportation</span><span class="sxs-lookup"><span data-stu-id="bc1d8-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="bc1d8-106">Cela peut être dû à certains filtres de sécurité de conformité qui ont été configurés par un administrateur spécifique et qui n’ont pas été communiqués à tous les administrateurs.</span><span class="sxs-lookup"><span data-stu-id="bc1d8-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="bc1d8-107">Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité susceptibles d’être à l’origine des problèmes suivants :</span><span class="sxs-lookup"><span data-stu-id="bc1d8-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="bc1d8-108">Connexion au centre de sécurité et de conformité PowerShell</span><span class="sxs-lookup"><span data-stu-id="bc1d8-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="bc1d8-109">Exécutez l’cmdlets suivante :</span><span class="sxs-lookup"><span data-stu-id="bc1d8-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="bc1d8-110">Pour plus d’informations sur les filtres de sécurité de conformité, consultez la rubrique [filtrage des autorisations pour la recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="bc1d8-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
