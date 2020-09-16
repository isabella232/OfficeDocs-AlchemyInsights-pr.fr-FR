---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734304"
---
# <a name="verify-your-domain"></a><span data-ttu-id="2f315-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="2f315-102">Verify your domain</span></span>

 <span data-ttu-id="2f315-103">**L’enregistrement n’a probablement pas été mis à jour sur Internet.**</span><span class="sxs-lookup"><span data-stu-id="2f315-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="2f315-104">En règle générale, il ne prend que quelques minutes pour pouvoir voir le nouvel enregistrement, mais il peut arriver que quelques heures se soient nécessaires.</span><span class="sxs-lookup"><span data-stu-id="2f315-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="2f315-105">Si vous avez attendu une fois déjà, vérifiez que vous avez copié et collé la valeur exacte dans l’enregistrement de vérification TXT au niveau de votre hôte DNS.</span><span class="sxs-lookup"><span data-stu-id="2f315-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="2f315-106">Le problème vient souvent de l'omission de la portion « MS= » de l'enregistrement.</span><span class="sxs-lookup"><span data-stu-id="2f315-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="2f315-107">Celle-ci est indispensable.</span><span class="sxs-lookup"><span data-stu-id="2f315-107">We need that too!</span></span>

- <span data-ttu-id="2f315-108">Pour certains hôtes DNS, une étape supplémentaire est nécessaire pour enregistrer le fichier de zone (emplacement de stockage de l'enregistrement DNS) de façon à ce qu'il soit mis à jour sur Internet.</span><span class="sxs-lookup"><span data-stu-id="2f315-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="2f315-109">Assurez-vous que vous avez enregistré vos modifications afin que Microsoft puisse voir et vérifier l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="2f315-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
