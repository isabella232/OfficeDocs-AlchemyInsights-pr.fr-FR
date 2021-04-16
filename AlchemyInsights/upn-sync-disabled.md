---
title: Synchronisation UPN désactivée
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782149"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="a905a-102">Synchronisation UPN désactivée</span><span class="sxs-lookup"><span data-stu-id="a905a-102">UPN sync disabled</span></span>

<span data-ttu-id="a905a-103">Si vous avez commencé la synchronisation avec Azure AD avant le 30 mars 2016, exécutez l'cmdlet Azure AD PowerShell suivante pour activer la correspondance souple UPN pour votre organisation uniquement :</span><span class="sxs-lookup"><span data-stu-id="a905a-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="a905a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="a905a-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="a905a-105">La correspondance avec le nom d'upn soft est automatiquement désactivée pour les organisations qui ont commencé à se synchroniser avec Azure AD le 30 mars 2016 ou après.</span><span class="sxs-lookup"><span data-stu-id="a905a-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="a905a-106">Pour en savoir plus sur l'activation de la correspondance souple sur UPN et d'autres fonctionnalités de synchronisation, consultez les fonctionnalités du service de [synchronisation Azure AD Connect.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="a905a-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

