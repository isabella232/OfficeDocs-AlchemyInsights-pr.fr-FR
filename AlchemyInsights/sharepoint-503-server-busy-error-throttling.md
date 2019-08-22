---
title: Limitation de SharePoint Online
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559839"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="e2f8d-102">Limitation de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e2f8d-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="e2f8d-103">Les utilisateurs peuvent recevoir un message d’erreur «le serveur 503 est occupé» lors de la tentative de navigation vers des sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="e2f8d-104">Cette erreur peut être causée par la limitation dans le service SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="e2f8d-105">SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="e2f8d-106">Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="e2f8d-107">Si vous effectuez l'obtenir limitées, 99 % du temps il s'agit en raison d'un code personnalisé.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="e2f8d-108">Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="e2f8d-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="e2f8d-109">Si vous pensez que cette erreur n’est pas liée à la limitation, vous pouvez vérifier si la maintenance active a lieu sur votre client en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="e2f8d-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="e2f8d-110">Enfin, vous devez consulter la page [État du service](https://portal.office.com/adminportal/home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire.</span><span class="sxs-lookup"><span data-stu-id="e2f8d-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

