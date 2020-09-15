---
title: Problèmes liés à l’intégration d’ordinateurs
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676880"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="27205-102">Problèmes liés à l’intégration d’ordinateurs</span><span class="sxs-lookup"><span data-stu-id="27205-102">Issues with onboarding machines</span></span>

<span data-ttu-id="27205-103">Il se peut que vous rencontriez des problèmes avec l’intégration d’ordinateurs au service MDATP.</span><span class="sxs-lookup"><span data-stu-id="27205-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="27205-104">Si vous pouvez accéder à l’ordinateur de l’utilisateur final, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="27205-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="27205-105">Téléchargez l’outil de diagnostic [Analyseur de connectivité client](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="27205-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="27205-106">Faites l’extraction et exécutez MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="27205-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="27205-107">Localisez le journal de diagnostic dans le dossier nommé MDATPClientAnalyzerResult, dossier identique à celui dans lequel l’outil Analyseur est téléchargé.</span><span class="sxs-lookup"><span data-stu-id="27205-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="27205-108">Examinez le fichier du journal, MDATPClientAnalyzer.txt, pour rechercher les problèmes de connectivité ou de paramètres de proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="27205-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>