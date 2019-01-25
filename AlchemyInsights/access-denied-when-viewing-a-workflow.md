---
title: Accès refusé lors de l’affichage d’un flux de travail
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468816"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="15fc9-102">Accès refusé lors de l’affichage d’un flux de travail</span><span class="sxs-lookup"><span data-stu-id="15fc9-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="15fc9-103">Flux de travail SharePoint 2013 qui tentent d’envoyer un message électronique à un groupe SharePoint peut échouer avec un message d’erreur « Accès refusé » si l’appartenance au groupe SharePoint n’est pas défini sur tout le monde.</span><span class="sxs-lookup"><span data-stu-id="15fc9-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="15fc9-104">**Pour résoudre ce problème, procédez comme suit :**</span><span class="sxs-lookup"><span data-stu-id="15fc9-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="15fc9-105">Autoriser tout le monde afficher les membres du groupe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="15fc9-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="15fc9-106">Supprimer du groupe SharePoint dans les zones à ou CC ligne du courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="15fc9-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="15fc9-107">Ajoutez explicitement les utilisateurs pour le champ à ou CC de ligne si la visibilité de l’appartenance ne peut pas être modifiée pour un groupe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="15fc9-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="15fc9-108">Pour afficher plus d’informations, consultez [HTTP non autorisés à /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="15fc9-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

