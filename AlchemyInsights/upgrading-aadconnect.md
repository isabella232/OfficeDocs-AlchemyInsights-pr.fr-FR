---
title: 932 mise à niveau de AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778740"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="a0c65-102">Mettre à niveau Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="a0c65-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="a0c65-103">Par défaut, la mise à niveau automatique est activée pour Azure AD Connect, ce qui permet de s'assurer que vous utilisez la dernière version.</span><span class="sxs-lookup"><span data-stu-id="a0c65-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="a0c65-104">Pour vérifier les paramètres de mise à niveau automatique, utilisez la cmdlet **Get-ADSyncAutoUpgrade** dans Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a0c65-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="a0c65-105">L'applet de commande renvoie l'une des valeurs suivantes:</span><span class="sxs-lookup"><span data-stu-id="a0c65-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="a0c65-106">**Activé**: la mise à niveau automatique est activée.</span><span class="sxs-lookup"><span data-stu-id="a0c65-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="a0c65-107">**Désactivé**: la mise à niveau automatique est désactivée.</span><span class="sxs-lookup"><span data-stu-id="a0c65-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="a0c65-108">**Suspendu**: le système n'est plus autorisé à recevoir des mises à niveau automatiques.</span><span class="sxs-lookup"><span data-stu-id="a0c65-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="a0c65-109">Vous ne pouvez pas configurer cette valeur; elle est définie par le système.</span><span class="sxs-lookup"><span data-stu-id="a0c65-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="a0c65-110">Pour plus d'informations, consultez la rubrique [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="a0c65-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="a0c65-111">Pour télécharger la dernière version d'Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="a0c65-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

