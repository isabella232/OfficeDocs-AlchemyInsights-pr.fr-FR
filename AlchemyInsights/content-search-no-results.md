---
title: Recherche de contenu sans résultats
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816846"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="59154-102">Aucun résultat de recherche/exportation de contenu</span><span class="sxs-lookup"><span data-stu-id="59154-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="59154-103">Les problèmes de recherche/exportation de contenu ne renvoyant aucune donnée peuvent être dus à un certain filtre de sécurité de conformité configuré par un administrateur spécifique et qui n’a pas été communiqué à tous les administrateurs.</span><span class="sxs-lookup"><span data-stu-id="59154-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="59154-104">Pour résoudre ce problème, vérifiez s’il existe des filtres de sécurité de conformité qui peuvent être à l’origine de ce problème :</span><span class="sxs-lookup"><span data-stu-id="59154-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="59154-105">Se connecter au Centre de sécurité et conformité PowerShell</span><span class="sxs-lookup"><span data-stu-id="59154-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="59154-106">Exécutez les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="59154-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="59154-107">$org = « yourdomain.com »</span><span class="sxs-lookup"><span data-stu-id="59154-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="59154-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="59154-108">Get-ComplianceSecurityFilter -Organization $org</span></span>