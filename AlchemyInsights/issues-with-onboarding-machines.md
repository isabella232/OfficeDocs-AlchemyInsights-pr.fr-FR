---
title: Problèmes liés à l’intégration d’ordinateurs
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139024"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="e55a0-102">Problèmes liés à l’intégration d’ordinateurs</span><span class="sxs-lookup"><span data-stu-id="e55a0-102">Issues with onboarding machines</span></span>

<span data-ttu-id="e55a0-103">Il se peut que vous rencontriez des problèmes avec l’intégration d’ordinateurs au service MDATP.</span><span class="sxs-lookup"><span data-stu-id="e55a0-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="e55a0-104">Si vous pouvez accéder à l’ordinateur de l’utilisateur final, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="e55a0-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="e55a0-105">Téléchargez l’outil de diagnostic [Analyseur de connectivité client](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="e55a0-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="e55a0-106">Faites l’extraction et exécutez MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="e55a0-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="e55a0-107">Localisez le journal de diagnostic dans le dossier nommé MDATPClientAnalyzerResult, dossier identique à celui dans lequel l’outil Analyseur est téléchargé.</span><span class="sxs-lookup"><span data-stu-id="e55a0-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="e55a0-108">Examinez le fichier du journal, MDATPClientAnalyzer.txt, pour rechercher les problèmes de connectivité ou de paramètres de proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="e55a0-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>