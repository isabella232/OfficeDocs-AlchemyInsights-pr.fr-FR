---
title: Modifier les serveurs de noms
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 148fbee1c14a8da6ede5ec5ccae90b1a4340ce32
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363075"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="34a0f-102">Mettre à jour les serveurs de noms de votre domaine vers Office 365</span><span class="sxs-lookup"><span data-stu-id="34a0f-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="34a0f-103">Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="34a0f-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="34a0f-p101">Pour configurer votre domaine dans Office 365, les serveurs de noms de votre bureau d’enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d’enregistrement de domaine.</span><span class="sxs-lookup"><span data-stu-id="34a0f-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="34a0f-106">Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="34a0f-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="34a0f-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="34a0f-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="34a0f-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="34a0f-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="34a0f-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="34a0f-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="34a0f-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="34a0f-110">Save changes.</span></span>

<span data-ttu-id="34a0f-111">Vous trouverez également des instructions détaillées dans cet article : [Modifier les serveurs de noms de manière à configurer Office 365 avec n’importe quel bureau d’enregistrement de domaines](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="34a0f-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  