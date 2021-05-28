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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657927"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="684d9-102">Configurer le point de terminaison DLP</span><span class="sxs-lookup"><span data-stu-id="684d9-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="684d9-103">Microsoft Endpoint DLP vous permet d’étendre la protection et la fonctionnalité de surveillance de DLP aux informations sensibles sur les appareils Windows 10.</span><span class="sxs-lookup"><span data-stu-id="684d9-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="684d9-104">Une fois que les appareils sont intégrés à la gestion des appareils, vous pouvez créer des stratégies DLP afin d’appliquer des actions de protection sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="684d9-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="684d9-105">L’Explorateur d’activités peut être utilisé pour surveiller l’activité des éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="684d9-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="684d9-106">Pour plus d’informations, consultez [Appareils d’intégration dans la gestion des appareils](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="684d9-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="684d9-107">Pour commencer à utiliser point de terminaison DLP :</span><span class="sxs-lookup"><span data-stu-id="684d9-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="684d9-108">Vérifiez que vous disposez des licences SKU/abonnements appropriées.</span><span class="sxs-lookup"><span data-stu-id="684d9-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="684d9-109">Pour plus d’informations, consultez [Licences SKU/abonnements](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="684d9-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="684d9-110">Vérifiez les autorisations requises pour activer la gestion des appareils, accéder à la page d’intégration ou activer/désactiver la surveillance de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="684d9-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="684d9-111">Pour plus d’informations, consultez [Autorisations](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="684d9-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="684d9-112">Intégrez des appareils dans la gestion des appareils en suivant la procédure sur les appareils d’intégration.</span><span class="sxs-lookup"><span data-stu-id="684d9-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="684d9-113">Pour plus d’informations, consultez [Appareils d’intégration](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="684d9-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="684d9-114">Créez des stratégies DLP pour protéger vos éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="684d9-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="684d9-115">Pour plus d’informations [Scénarios de stratégie DLP pour les points de terminaison](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="684d9-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="684d9-116">Pour plus d’informations sur le point de terminaison Microsoft DLP, consultez [En savoir plus sur les points de terminaison de protection contre la perte de données Microsoft 365 (préversion)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="684d9-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="684d9-117">**Étapes importantes de la collecte de données si une prise en charge est nécessaire :**</span><span class="sxs-lookup"><span data-stu-id="684d9-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="684d9-118">Téléchargez [La version préliminaire de l’analyseur de client MDATP](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="684d9-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="684d9-119">Exécutez l’outil en tant qu’administrateur à partir de la fenêtre cmd :</span><span class="sxs-lookup"><span data-stu-id="684d9-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="684d9-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="684d9-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="684d9-121">Lorsque vous êtes invité par cette note **Entrez le nombre de minutes pour collecter les traces**, entrez le nombre de minutes nécessaires pour exécuter le scénario.</span><span class="sxs-lookup"><span data-stu-id="684d9-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="684d9-122">Exécuter le scénario.</span><span class="sxs-lookup"><span data-stu-id="684d9-122">Run the scenario.</span></span>

<span data-ttu-id="684d9-123">Collectez la sortie du fichier zip à remettre à l'agent de support.</span><span class="sxs-lookup"><span data-stu-id="684d9-123">Collect the Zip file output to give to the Support agent.</span></span>
