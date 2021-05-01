---
title: Dépannage du blocage de la tâche du service d’importation
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059844"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="b611c-102">Dépannage du blocage de la tâche du service d’importation</span><span class="sxs-lookup"><span data-stu-id="b611c-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="b611c-103">Si vous rencontrez des problèmes avec des tâches de service d’importation bloquées ou défaillantes, examinez et essayez ceci :</span><span class="sxs-lookup"><span data-stu-id="b611c-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="b611c-104">Examinez la taille du fichier PST.</span><span class="sxs-lookup"><span data-stu-id="b611c-104">Review the size of of the PST file.</span></span> <span data-ttu-id="b611c-105">La taille maximale recommandée d’un fichier PST pour l’importation est de 20 Go.</span><span class="sxs-lookup"><span data-stu-id="b611c-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="b611c-106">Si vous pensez que des éléments ont été ignorés en raison d’une corruption, exécutez Scanpst.exe pour diagnostiquer et corriger les erreurs dans les fichiers PST.</span><span class="sxs-lookup"><span data-stu-id="b611c-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="b611c-107">Si vous voyez une erreur « MapiExceptionShutoffÉléceed » lors de l’importation, assurez-vous que la boîte aux lettres cible dispose des capacités suffisantes pour importer les fichiers PST souhaités.</span><span class="sxs-lookup"><span data-stu-id="b611c-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="b611c-108">Pour plus d’informations sur la résolution des problèmes liés à la tâche d’importation de données PST, consultez [Résoudre les problèmes liés aux tâches d’importation PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="b611c-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="b611c-109">Pour plus d’informations sur la correction des problèmes lors de l’importation de fichiers PST dans Outlook, consultez [Résoudre les problèmes d’importation d’un fichier .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="b611c-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>