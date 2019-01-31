---
title: Mettre à jour les serveurs de noms de votre domaine vers Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 16821181a58da470b37e286e082180d0c6012b2d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655845"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="068df-102">Mettre à jour les serveurs de noms de votre domaine vers Office 365</span><span class="sxs-lookup"><span data-stu-id="068df-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="068df-103">Remarque : Les modifications du serveur de noms peuvent parfois prendre jusqu'à 48 heures pour propager.</span><span class="sxs-lookup"><span data-stu-id="068df-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="068df-p101">Pour configurer votre domaine dans Office 365, les serveurs de noms de votre bureau d'enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d'enregistrement de domaine.</span><span class="sxs-lookup"><span data-stu-id="068df-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="068df-106">Accédez au site web de votre bureau d'enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="068df-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="068df-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="068df-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="068df-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="068df-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="068df-109">NS2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="068df-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="068df-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="068df-110">Save changes.</span></span>
    
<span data-ttu-id="068df-111">Vous trouverez également des instructions détaillées dans cet article : [Modifier les serveurs de noms de manière à configurer Office 365 avec n'importe quel bureau d'enregistrement de domaines](https://support.office.com/article/https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="068df-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

