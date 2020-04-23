---
title: Modifier les serveurs de noms
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706753"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="975eb-102">Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft</span><span class="sxs-lookup"><span data-stu-id="975eb-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="975eb-103">Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="975eb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="975eb-p101">Pour configurer votre domaine dans Microsoft 365, les serveurs de noms de votre bureau d’enregistrement doivent être mis à jour. Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d’enregistrement de domaines.</span><span class="sxs-lookup"><span data-stu-id="975eb-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="975eb-106">Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="975eb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="975eb-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="975eb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="975eb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="975eb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="975eb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="975eb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="975eb-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="975eb-110">Save changes.</span></span>

<span data-ttu-id="975eb-111">Vous trouverez également des instructions détaillées dans cet article : [Modifier les serveurs de noms avec n’importe quel bureau d’enregistrement de domaines](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="975eb-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  