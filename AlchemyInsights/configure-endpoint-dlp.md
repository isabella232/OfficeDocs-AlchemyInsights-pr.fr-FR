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
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812113"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="95c17-102">Configurer le point de terminaison DLP</span><span class="sxs-lookup"><span data-stu-id="95c17-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="95c17-103">Microsoft Endpoint DLP vous permet d’étendre la protection et la fonctionnalité de surveillance de DLP aux informations sensibles sur les appareils Windows 10.</span><span class="sxs-lookup"><span data-stu-id="95c17-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="95c17-104">Une fois que les appareils sont intégrés à la gestion des appareils, vous pouvez créer des stratégies DLP afin d’appliquer des actions de protection sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="95c17-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="95c17-105">L’Explorateur d’activités peut être utilisé pour surveiller l’activité des éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="95c17-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="95c17-106">Pour plus d’informations, consultez [Appareils d’intégration dans la gestion des appareils](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="95c17-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="95c17-107">Pour commencer à utiliser point de terminaison DLP :</span><span class="sxs-lookup"><span data-stu-id="95c17-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="95c17-108">Vérifiez que vous disposez des licences SKU/abonnements appropriées.</span><span class="sxs-lookup"><span data-stu-id="95c17-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="95c17-109">Pour plus d’informations, consultez [Licences SKU/abonnements](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="95c17-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="95c17-110">Vérifiez les autorisations requises pour activer la gestion des appareils, accéder à la page d’intégration ou activer/désactiver la surveillance de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="95c17-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="95c17-111">Pour plus d’informations, consultez [Autorisations](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="95c17-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="95c17-112">Intégrez des appareils dans la gestion des appareils en suivant la procédure sur les appareils d’intégration.</span><span class="sxs-lookup"><span data-stu-id="95c17-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="95c17-113">Si vous ne disposez pas de l’option d’intégration d’appareils (préversion) sous **Paramètres** de conformité M365, confirmez que vous disposez de la licence et des autorisations appropriées mentionnées ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="95c17-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="95c17-114">Pour plus d’informations, consultez [Appareils d’intégration](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="95c17-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="95c17-115">Créez des stratégies DLP pour protéger vos éléments sensibles.</span><span class="sxs-lookup"><span data-stu-id="95c17-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="95c17-116">Pour plus d’informations [Scénarios de stratégie DLP pour les points de terminaison](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="95c17-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="95c17-117">Pour plus d’informations sur le point de terminaison Microsoft DLP, consultez [En savoir plus sur les points de terminaison de protection contre la perte de données Microsoft 365 (préversion)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="95c17-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>