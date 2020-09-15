---
title: Conflits avec SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 877c954bea219cf8d885645cd25e41a5b7bab6fd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713452"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="bc60b-102">Conflits avec SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc60b-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="bc60b-103">Si des messages d’erreur s’affichent pendant la synchronisation, tels que « Un objet synchronisé avec la même ProxyAddress ou le même UserPrincipalName existe dans votre répertoire », consultez [Diagnostiquer les erreurs de synchronisation d’attributs dupliqués et y remédier](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="bc60b-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="bc60b-104">Vous pouvez également activer la résilience des attributs en double.</span><span class="sxs-lookup"><span data-stu-id="bc60b-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="bc60b-105">Pour en savoir plus, consultez [Identifier la synchronisation et dupliquer la résilience de l’attribut](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="bc60b-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>