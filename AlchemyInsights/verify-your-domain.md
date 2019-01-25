---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29469202"
---
# <a name="verify-your-domain"></a><span data-ttu-id="5bcce-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="5bcce-102">Verify your domain</span></span>

 <span data-ttu-id="5bcce-103">**L’enregistrement n’a pas probablement mis à jour sur Internet.**</span><span class="sxs-lookup"><span data-stu-id="5bcce-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="5bcce-104">En règle générale ne prend quelques minutes pour nous être en mesure de voir le nouvel enregistrement, mais peut parfois prendre que quelques heures.</span><span class="sxs-lookup"><span data-stu-id="5bcce-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="5bcce-p101">Si vous avez attendu qui long déjà, vérifiez que vous avez copié et collé la valeur exacte dans l’enregistrement de vérification TXT à votre hôte DNS. Un problème courant n’inclut pas la « MS = » fait partie de l’enregistrement. Nous avons besoin que trop !</span><span class="sxs-lookup"><span data-stu-id="5bcce-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="5bcce-p102">Vous devez effectuer une étape supplémentaire pour enregistrer le fichier de zone (où est stocké l’enregistrement DNS) à certains hôtes DNS, afin qu’il met à jour sur Internet. Assurez-vous que vous avez enregistré vos modifications Office 365 peuvent se voir et vérifier l’enregistrement.</span><span class="sxs-lookup"><span data-stu-id="5bcce-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

