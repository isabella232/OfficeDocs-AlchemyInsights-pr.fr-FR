---
title: Verify your domain
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
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770989"
---
# <a name="verify-your-domain"></a><span data-ttu-id="fcb2e-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="fcb2e-102">Verify your domain</span></span>

 <span data-ttu-id="fcb2e-103">**L'enregistrement n'a probablement pas été mis à jour sur Internet.**</span><span class="sxs-lookup"><span data-stu-id="fcb2e-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="fcb2e-104">En règle générale, nous ne pouvons voir le nouvel enregistrement que quelques minutes, mais cela peut parfois prendre jusqu'à quelques heures.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="fcb2e-105">Si vous avez attendu aussi longtemps, vérifiez que vous avez copié et copié la valeur exacte dans l'enregistrement de vérification TXT de votre hôte DNS.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="fcb2e-106">Le problème vient souvent de l'omission de la portion « MS= » de l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="fcb2e-107">Celle-ci est indispensable.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-107">We need that too!</span></span>

- <span data-ttu-id="fcb2e-108">Pour certains hôtes DNS, une étape supplémentaire est nécessaire pour enregistrer le fichier de zone (emplacement de stockage de l'enregistrement DNS) de façon à ce qu'il soit mis à jour sur Internet.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="fcb2e-109">Vérifiez que vous avez enregistré vos modifications afin que Microsoft puisse voir et vérifier l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="fcb2e-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
