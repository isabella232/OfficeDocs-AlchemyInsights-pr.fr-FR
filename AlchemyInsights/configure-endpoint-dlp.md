---
title: Configurer le point de terminaison DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402419"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f2dd0-102">Configurer le point de terminaison DLP</span><span class="sxs-lookup"><span data-stu-id="f2dd0-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f2dd0-103">Microsoft Endpoint DLP vous permet d’étendre la protection et la fonctionnalité de surveillance de DLP aux informations sensibles sur les appareils Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f2dd0-104">Une fois que les appareils sont intégrés à la gestion des appareils, vous pouvez créer des stratégies DLP afin d’appliquer des actions de protection sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f2dd0-105">L’Explorateur d’activités peut être utilisé pour surveiller l’activité des éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f2dd0-106">Pour plus d’informations, consultez [Appareils d’intégration dans la gestion des appareils](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f2dd0-107">Pour commencer à utiliser point de terminaison DLP :</span><span class="sxs-lookup"><span data-stu-id="f2dd0-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f2dd0-108">Vérifiez que vous disposez des licences SKU/abonnements appropriées.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f2dd0-109">Pour plus d’informations, consultez [Licences SKU/abonnements](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f2dd0-110">Vérifiez les autorisations requises pour activer la gestion des appareils, accéder à la page d’intégration ou activer/désactiver la surveillance de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="f2dd0-111">Pour plus d’informations, consultez [Autorisations](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f2dd0-112">Intégrez des appareils dans la gestion des appareils en suivant la procédure sur les appareils d’intégration.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f2dd0-113">Si vous ne disposez pas de l’option d’intégration d’appareils (préversion) sous **Paramètres** de conformité M365, confirmez que vous disposez de la licence et des autorisations appropriées mentionnées ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="f2dd0-114">Pour plus d’informations, consultez [Appareils d’intégration](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f2dd0-115">Créez des stratégies DLP pour protéger vos éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f2dd0-116">Pour plus d’informations [Scénarios de stratégie DLP pour les points de terminaison](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="f2dd0-117">Pour plus d’informations sur le point de terminaison Microsoft DLP, consultez [En savoir plus sur les points de terminaison de protection contre la perte de données Microsoft 365 (préversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="f2dd0-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f2dd0-118">**Étapes importantes de la collecte de données si une prise en charge est nécessaire :**</span><span class="sxs-lookup"><span data-stu-id="f2dd0-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f2dd0-119">Téléchargez l'aperçu du MDATP Client Analyzer sur [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="f2dd0-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="f2dd0-120">Exécutez l’outil en tant qu’administrateur à partir de la fenêtre cmd :</span><span class="sxs-lookup"><span data-stu-id="f2dd0-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="f2dd0-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="f2dd0-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="f2dd0-122">Lorsque le message « Entrez le nombre de minutes pour collecter les traces » vous est demandé : entrez le nombre de minutes nécessaires pour exécuter le scénario</span><span class="sxs-lookup"><span data-stu-id="f2dd0-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="f2dd0-123">Exécuter le scénario</span><span class="sxs-lookup"><span data-stu-id="f2dd0-123">Run the scenario</span></span>

<span data-ttu-id="f2dd0-124">Collectez la sortie du fichier zip à remettre à l'agent de support.</span><span class="sxs-lookup"><span data-stu-id="f2dd0-124">Collect the Zip file output to be given to the Support agent.</span></span>
