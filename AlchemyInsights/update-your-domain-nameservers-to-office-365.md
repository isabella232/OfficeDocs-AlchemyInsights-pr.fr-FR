---
title: Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734909"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="7c632-102">Mettre à jour vos serveurs de noms de votre domaine de manière à ce qu’ils pointent vers Microsoft</span><span class="sxs-lookup"><span data-stu-id="7c632-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="7c632-103">Remarque : le Serveur de noms modifications peut prendre jusqu'à 48 heures.</span><span class="sxs-lookup"><span data-stu-id="7c632-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7c632-104">Pour configurer votre domaine avec Microsoft, les serveurs de noms de votre serveur d’inscriptions doivent être mis à jour.</span><span class="sxs-lookup"><span data-stu-id="7c632-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7c632-105">Créez ou modifiez vos enregistrements de serveur de noms auprès de votre bureau d'enregistrement de domaine.</span><span class="sxs-lookup"><span data-stu-id="7c632-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7c632-106">Accédez au site web de votre bureau d’enregistrement de domaines et recherchez la zone dans laquelle vous pouvez modifier les serveurs de noms.</span><span class="sxs-lookup"><span data-stu-id="7c632-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="7c632-107">Créez ou modifiez deux enregistrements de serveur de noms avec ces valeurs :</span><span class="sxs-lookup"><span data-stu-id="7c632-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7c632-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7c632-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7c632-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7c632-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7c632-110">Enregistrez les modifications.</span><span class="sxs-lookup"><span data-stu-id="7c632-110">Save changes.</span></span>

<span data-ttu-id="7c632-111">Vous trouverez également des instructions détaillées dans cet article : [modifier les serveurs de noms pour configurer Microsoft 365 avec n’importe quel bureau](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) d’enregistrement de domaines</span><span class="sxs-lookup"><span data-stu-id="7c632-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  