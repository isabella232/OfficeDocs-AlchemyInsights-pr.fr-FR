---
title: Mettre à jour les serveurs de noms de votre domaine vers Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 2447a3300782204b32d3c47325e1e987f6168be7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506045"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e6abe-102">Mettre à jour les serveurs de noms de votre domaine vers Office 365</span><span class="sxs-lookup"><span data-stu-id="e6abe-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e6abe-103">Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="e6abe-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e6abe-p101">Pour configurer votre domaine dans Office 365, les serveurs de noms de votre bureau d’enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d’enregistrement de domaine.</span><span class="sxs-lookup"><span data-stu-id="e6abe-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e6abe-106">Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="e6abe-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="e6abe-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="e6abe-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e6abe-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e6abe-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e6abe-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e6abe-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e6abe-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="e6abe-110">Save changes.</span></span>

<span data-ttu-id="e6abe-111">Vous trouverez également des instructions détaillées dans cet article : [Modifier les serveurs de noms de manière à configurer Office 365 avec n’importe quel bureau d’enregistrement de domaines](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="e6abe-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  