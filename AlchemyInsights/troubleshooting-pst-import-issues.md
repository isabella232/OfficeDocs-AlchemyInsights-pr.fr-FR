---
title: Résolution de problèmes d’importation PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059813"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="0d8eb-102">Résolution de problèmes d’importation PST</span><span class="sxs-lookup"><span data-stu-id="0d8eb-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="0d8eb-103">Si vous effectuez l’importation dans le client Outlook lui-même, consultez [Résoudre les problèmes d’importation d’un fichier .pst Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="0d8eb-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="0d8eb-104">Si vous utilisez le service d’importation et que celui-ci est bloqué, veuillez noter que la taille de chaque fichier PST chargé vers l’emplacement de stockage Azure ne doit pas dépasser 20 Go.</span><span class="sxs-lookup"><span data-stu-id="0d8eb-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="0d8eb-105">Les fichiers PST d’une taille supérieure à 20 Go peuvent avoir un impact sur les performances du processus d’importation PST.</span><span class="sxs-lookup"><span data-stu-id="0d8eb-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="0d8eb-106">Pour plus d’informations sur la résolution des problèmes de tâches bloquées, consultez les [problèmes qui affectent les tâches d’importation PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="0d8eb-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="0d8eb-107">Si vous voulez vérifier l’état d’une tâche spécifique d’importation, vous pouvez utiliser [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="0d8eb-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="0d8eb-108">Pour plus d’informations sur le service d’importation, consultez la [Vue d’ensemble de l’importation des fichiers PST de votre organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0d8eb-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
