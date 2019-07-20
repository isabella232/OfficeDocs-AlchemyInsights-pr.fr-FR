---
title: Recherche de contenu sans résultats
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800330"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="403d8-102">Aucun résultat de la recherche/exportation de contenu</span><span class="sxs-lookup"><span data-stu-id="403d8-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="403d8-103">Les problèmes liés à la recherche de contenu/exportation ne renvoyant pas de données peuvent être dus à un filtre de sécurité de conformité configuré par un administrateur spécifique et ne communiquant pas avec tous les administrateurs.</span><span class="sxs-lookup"><span data-stu-id="403d8-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="403d8-104">Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine du problème:</span><span class="sxs-lookup"><span data-stu-id="403d8-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="403d8-105">Connexion au centre de sécurité et de conformité PowerShell</span><span class="sxs-lookup"><span data-stu-id="403d8-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="403d8-106">Exécutez l’cmdlets suivante:</span><span class="sxs-lookup"><span data-stu-id="403d8-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="403d8-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="403d8-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="403d8-108">Get-ComplianceSecurityFilter-Organization $org</span><span class="sxs-lookup"><span data-stu-id="403d8-108">Get-ComplianceSecurityFilter -Organization $org</span></span>