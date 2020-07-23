---
title: Conflits avec SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186106"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="9183e-102">Conflits avec SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9183e-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="9183e-103">Si des messages d’erreur s’affichent pendant la synchronisation, tels que « Un objet synchronisé avec la même ProxyAddress ou le même UserPrincipalName existe dans votre répertoire », consultez [Diagnostiquer les erreurs de synchronisation d’attributs dupliqués et y remédier](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="9183e-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="9183e-104">Vous pouvez également activer la résilience des attributs en double.</span><span class="sxs-lookup"><span data-stu-id="9183e-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="9183e-105">Pour en savoir plus, consultez [Identifier la synchronisation et dupliquer la résilience de l’attribut](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="9183e-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>