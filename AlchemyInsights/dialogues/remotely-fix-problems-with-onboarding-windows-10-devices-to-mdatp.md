---
title: Résoudre à distance les problèmes liés à l’intégration d’appareils Windows 10 à Microsoft Defender - Protection avancée contre les menaces
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530007"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="7357d-102">Résoudre à distance les problèmes liés à l’intégration d’appareils Windows 10 à Microsoft Defender - Protection avancée contre les menaces</span><span class="sxs-lookup"><span data-stu-id="7357d-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="7357d-103">Si vous pouvez accéder à l’ordinateur distant, suivez les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="7357d-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="7357d-104">Téléchargez l’outil de diagnostic [Analyseur de connectivité client](https://go.microsoft.com/fwlink/?linkid=2143466).</span><span class="sxs-lookup"><span data-stu-id="7357d-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="7357d-105">Faites l’extraction et exécutez MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="7357d-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="7357d-106">Recherchez le journal de diagnostic dans le dossier MDATPClientAnalyzerResult, qui est le même dossier que celui dans lequel l’outil Analyzer a été téléchargé.</span><span class="sxs-lookup"><span data-stu-id="7357d-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="7357d-107">Pour rechercher des problèmes de connectivité ou de paramètres de proxy Internet, examinez le fichier journal MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="7357d-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="7357d-108">Pour plus d’informations, voir [Problèmes avec les ordinateurs d’intégration.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="7357d-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
