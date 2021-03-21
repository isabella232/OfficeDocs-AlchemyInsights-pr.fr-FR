---
title: Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901565"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="5e71d-102">Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison</span><span class="sxs-lookup"><span data-stu-id="5e71d-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="5e71d-103">Il se peut que vous rencontriez des problèmes avec l’intégration d’ordinateurs au service MDE.</span><span class="sxs-lookup"><span data-stu-id="5e71d-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="5e71d-104">Si vous pouvez accéder à l’ordinateur de l’utilisateur final, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="5e71d-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="5e71d-105">Téléchargez la dernière version d’évaluation de l’outil de diagnostic [Analyseur de client MDE](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="5e71d-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="5e71d-106">Cliquez avec le bouton droit sur **MDEClientAnalyzer.cmd**, puis sélectionnez « Exécuter en tant qu’administrateur ».</span><span class="sxs-lookup"><span data-stu-id="5e71d-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="5e71d-107">Suivez les instructions suggérées dans **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="5e71d-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="5e71d-108">Pour consulter des journaux plus détaillés, examinez le sous-dossier créé nommé **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="5e71d-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="5e71d-109">Si des instructions supplémentaires sont nécessaires, contactez le [Support Microsoft Defender pour point de terminaison](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) et fournissez le fichier MDEClientAnalysult.zip résultant pour analyse.</span><span class="sxs-lookup"><span data-stu-id="5e71d-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
