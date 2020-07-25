---
title: Stratégie de protection des applications
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266434"
---
# <a name="application-protection-policy"></a><span data-ttu-id="c5f74-102">Stratégie de protection des applications</span><span class="sxs-lookup"><span data-stu-id="c5f74-102">Application protection policy</span></span>

<span data-ttu-id="c5f74-103">Si vous débutez sur la stratégie de protection des applications, consultez la [Vue d’ensemble des stratégies de protection des applications](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="c5f74-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="c5f74-104">Pour commencer à utiliser l’application, consultez [Guide pratique de gestion et affectation des stratégies de protection des applications](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="c5f74-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="c5f74-105">Configuration requise pour la stratégie de protection des applications :</span><span class="sxs-lookup"><span data-stu-id="c5f74-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="c5f74-106">Un utilisateur a une licence Intune ou EMS.</span><span class="sxs-lookup"><span data-stu-id="c5f74-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="c5f74-107">L’utilisateur appartient à un groupe ciblé par les stratégies de protection des applications.</span><span class="sxs-lookup"><span data-stu-id="c5f74-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="c5f74-108">Un seul utilisateur d’entreprise est connecté aux applications protégées sur un appareil.</span><span class="sxs-lookup"><span data-stu-id="c5f74-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="c5f74-109">L’application a implémenté le [Kit de développement logiciel de Intune](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="c5f74-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="c5f74-110">Pour obtenir la liste des applications qui prennent en charge le SDK, consultez [Applications protégées Microsoft Intune](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="c5f74-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="c5f74-111">Les stratégies s’appliquent une fois qu’un utilisateur répondant aux conditions ci-dessus se connecte à une application Intune du kit de développement logiciel compatible.</span><span class="sxs-lookup"><span data-stu-id="c5f74-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="c5f74-112">La façon la plus simple de déterminer si une stratégie est appliquée est d’exiger que l’utilisateur définisse un code confidentiel dans la stratégie.</span><span class="sxs-lookup"><span data-stu-id="c5f74-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="c5f74-113">Pour plus d’informations, voir :</span><span class="sxs-lookup"><span data-stu-id="c5f74-113">For more information, see:</span></span>

[<span data-ttu-id="c5f74-114">Forum aux questions sur l’application/GAM</span><span class="sxs-lookup"><span data-stu-id="c5f74-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="c5f74-115">Valider la configuration de votre stratégie de protection des applications</span><span class="sxs-lookup"><span data-stu-id="c5f74-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="c5f74-116">Comprendre le minutage de la remise des stratégies de protection des applications</span><span class="sxs-lookup"><span data-stu-id="c5f74-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="c5f74-117">Comment surveiller les stratégies de protection des applications</span><span class="sxs-lookup"><span data-stu-id="c5f74-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)