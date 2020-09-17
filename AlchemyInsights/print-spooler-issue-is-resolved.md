---
title: Le problème de spouleur d’impression est résolu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801839"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="1b2d2-102">Le problème de spouleur d’impression est résolu</span><span class="sxs-lookup"><span data-stu-id="1b2d2-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="1b2d2-103">Si votre appareil a été mis à jour avec Windows 10 **Système d’exploitation Build 19041.329**, vous avez peut-être remarqué un problème dans lequel certaines imprimantes n’ont pas pu être imprimées.</span><span class="sxs-lookup"><span data-stu-id="1b2d2-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="1b2d2-104">Il se peut que le spouleur d’impression génère une erreur ou se ferme de manière inattendue lors de la tentative d’impression et qu’aucune sortie ne provient de l’imprimante affectée.</span><span class="sxs-lookup"><span data-stu-id="1b2d2-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="1b2d2-105">Ce problème a été résolu dans la version dusystème d’exploitation **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="1b2d2-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="1b2d2-106">**Examen continu**</span><span class="sxs-lookup"><span data-stu-id="1b2d2-106">**Ongoing investigation**</span></span>

<span data-ttu-id="1b2d2-107">Le fichier LSASS (service de sous-système d’autorité de sécurité locale) (**isass.exe**) peut échouer sur certains appareils avec le message d’erreur « un processus système critique, C:\WINDOWS\system32\Isass.exe, a échoué avec le code d’État c0000008.</span><span class="sxs-lookup"><span data-stu-id="1b2d2-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="1b2d2-108">L’ordinateur doit maintenant être redémarré ».</span><span class="sxs-lookup"><span data-stu-id="1b2d2-108">The machine must now be restarted".</span></span>  <span data-ttu-id="1b2d2-109">**Microsoft travaille sur une résolution et fournit une mise à jour dans une prochaine publication.**</span><span class="sxs-lookup"><span data-stu-id="1b2d2-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="1b2d2-110">Pour plus d’informations, consultez [problèmes connus Windows 10 version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="1b2d2-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>