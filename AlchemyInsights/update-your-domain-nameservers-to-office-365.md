---
title: Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510282"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="e3e69-102">Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft</span><span class="sxs-lookup"><span data-stu-id="e3e69-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="e3e69-103">Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="e3e69-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e3e69-104">Pour configurer votre domaine avec Microsoft, les serveurs de noms de votre serveur d’inscriptions doivent être mis à jour.</span><span class="sxs-lookup"><span data-stu-id="e3e69-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e3e69-105">Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d'enregistrement de domaine.</span><span class="sxs-lookup"><span data-stu-id="e3e69-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e3e69-106">Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="e3e69-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="e3e69-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="e3e69-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e3e69-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e3e69-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e3e69-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e3e69-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e3e69-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="e3e69-110">Save changes.</span></span>

<span data-ttu-id="e3e69-111">Vous trouverez également des instructions détaillées dans cet article : [modifier les serveurs de noms pour configurer Microsoft 365 avec n’importe quel bureau](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) d’enregistrement de domaines</span><span class="sxs-lookup"><span data-stu-id="e3e69-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  