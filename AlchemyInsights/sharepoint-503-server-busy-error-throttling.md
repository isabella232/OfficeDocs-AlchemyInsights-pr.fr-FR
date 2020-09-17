---
title: Limitation de SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773845"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="2afe0-102">Limitation de SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2afe0-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="2afe0-103">**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.</span><span class="sxs-lookup"><span data-stu-id="2afe0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2afe0-104">**erreur de disponibilité du serveur 503**</span><span class="sxs-lookup"><span data-stu-id="2afe0-104">**503 server is busy error**</span></span>

<span data-ttu-id="2afe0-105">Les utilisateurs peuvent recevoir un message d’erreur « le serveur 503 est occupé » lors de la tentative de navigation vers des sites SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2afe0-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="2afe0-106">Cette erreur peut être causée par la limitation dans le service SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2afe0-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="2afe0-107">SharePoint Online utilise la limitation à mettre à jour d'optimiser les performances et la fiabilité du service SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2afe0-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="2afe0-108">Le nombre d'actions de l'utilisateur ou simultanés limitations appelle (par script ou code) pour éviter la surutilisation des ressources.</span><span class="sxs-lookup"><span data-stu-id="2afe0-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="2afe0-109">Pour plus d’informations sur la limitation, consultez la rubrique [éviter d’être limité ou bloqué dans SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2afe0-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="2afe0-110">Si vous pensez que cette erreur n’est pas liée à la limitation, vous pouvez vérifier si la maintenance active a lieu sur votre client en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="2afe0-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="2afe0-111">Enfin, vous devez consulter la page [État du service](https://portal.office.com/adminportal/home#/servicehealth) pour vérifier les avis/incidents susceptibles de se produire.</span><span class="sxs-lookup"><span data-stu-id="2afe0-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

