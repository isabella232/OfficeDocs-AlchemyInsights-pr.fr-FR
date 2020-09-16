---
title: Résoudre les problèmes de performances de OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757883"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="8fc22-102">Résoudre les problèmes de performances de OneDrive</span><span class="sxs-lookup"><span data-stu-id="8fc22-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="8fc22-103">Si vous rencontrez une synchronisation plus lente que prévu ou des problèmes de performances similaires avec OneDrive :</span><span class="sxs-lookup"><span data-stu-id="8fc22-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="8fc22-104">Vérifiez qu’il n’y a pas de problèmes connus à l’aide du [tableau de bord d’État du service](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8fc22-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="8fc22-105">[Activez les fichiers à la demande](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) afin de pouvoir accéder à tous vos fichiers dans OneDrive sans avoir à les télécharger tous et à utiliser l’espace de stockage sur votre appareil.</span><span class="sxs-lookup"><span data-stu-id="8fc22-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="8fc22-106">[Passez en revue les meilleures pratiques](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) pour la planification et les performances du réseau.</span><span class="sxs-lookup"><span data-stu-id="8fc22-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="8fc22-107">[Optimisez la vitesse](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)de téléchargement et de téléchargement, en particulier si vous synchronisez un appareil pour la première fois.</span><span class="sxs-lookup"><span data-stu-id="8fc22-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="8fc22-108">Si vous synchronisez une bibliothèque avec plus de 100 000 éléments, la synchronisation OneDrive peut sembler bloquée longtemps ou l’état indique le traitement de la 0KB de xMB. "</span><span class="sxs-lookup"><span data-stu-id="8fc22-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="8fc22-109">[En savoir plus sur la synchronisation de plus de 100 000 fichiers](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , ainsi que sur [la limite de 300 000 fichiers pris en charge par OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="8fc22-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="8fc22-p102">Lorsqu'un utilisateur dépasse les limites d'utilisation, SharePoint Online limitations des autres requêtes destinées à partir de ce compte d'utilisateur pour une courte période. Toutes les actions de l'utilisateur sont limitées alors que la limitation est en vigueur.</span><span class="sxs-lookup"><span data-stu-id="8fc22-p102">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period. All user actions are throttled while the throttle is in effect.</span></span>
