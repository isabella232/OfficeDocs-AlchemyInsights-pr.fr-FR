---
title: Accès refusé lors de l’affichage d’un flux de travail
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050523"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="396bc-102">Accès refusé lors de l’affichage d’un flux de travail</span><span class="sxs-lookup"><span data-stu-id="396bc-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="396bc-103">Les flux de travail SharePoint 2013 qui tentent d’envoyer un courrier électronique à un groupe SharePoint peuvent échouer avec un message d’erreur « Accès refusé » si l’appartenance au groupe SharePoint n’est pas définie sur tout le monde.</span><span class="sxs-lookup"><span data-stu-id="396bc-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="396bc-104">**Pour résoudre ce problème, procédez comme suit :**</span><span class="sxs-lookup"><span data-stu-id="396bc-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="396bc-105">Autoriser tout le monde à voir les membres du groupe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="396bc-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="396bc-106">Supprimez le groupe SharePoint de la ligne à ou CC du message électronique.</span><span class="sxs-lookup"><span data-stu-id="396bc-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="396bc-107">Ajoutez explicitement les utilisateurs à la ligne à ou CC si la visibilité de l’appartenance ne peut pas être modifiée pour le groupe SharePoint.</span><span class="sxs-lookup"><span data-stu-id="396bc-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="396bc-108">Pour plus d’informations, reportez-vous à la rubrique [http Unauthorized to/_vti_bin/client.svc/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="396bc-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  