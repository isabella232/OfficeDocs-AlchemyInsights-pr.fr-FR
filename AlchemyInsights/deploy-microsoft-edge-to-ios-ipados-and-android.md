---
title: Déployer Microsoft Edge sur iOS, iPadOS et Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177992"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="e285a-102">Déployer Microsoft Edge sur iOS, iPadOS et Android</span><span class="sxs-lookup"><span data-stu-id="e285a-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="e285a-103">Le scénario guidé résumé ci-dessous vous aide à affecter Microsoft Edge aux utilisateurs d’appareils iOS, iPadOS et Android.</span><span class="sxs-lookup"><span data-stu-id="e285a-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="e285a-104">Si vous avez bloqué l’inscription des utilisateurs sur les appareils mobiles, ce scénario guidé ne fonctionne pas et les utilisateurs devront installer Microsoft Edge eux-mêmes.</span><span class="sxs-lookup"><span data-stu-id="e285a-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="e285a-105">Le scénario guidé comprend les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="e285a-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="e285a-106">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="e285a-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="e285a-107">Introduction</span><span class="sxs-lookup"><span data-stu-id="e285a-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="e285a-108">Concepts de base</span><span class="sxs-lookup"><span data-stu-id="e285a-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="e285a-109">Configuration</span><span class="sxs-lookup"><span data-stu-id="e285a-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="e285a-110">Devoirs</span><span class="sxs-lookup"><span data-stu-id="e285a-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="e285a-111">Révision et création</span><span class="sxs-lookup"><span data-stu-id="e285a-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="e285a-112">Après avoir suivi les étapes du scénario guidé, les stratégies Microsoft Intune activeront les fonctionnalités suivantes de Microsoft Edge pour la productivité :</span><span class="sxs-lookup"><span data-stu-id="e285a-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="e285a-113">Identité double</span><span class="sxs-lookup"><span data-stu-id="e285a-113">Dual identity</span></span>
- <span data-ttu-id="e285a-114">Intégration à la stratégie de protection des applications Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e285a-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="e285a-115">Intégration au proxy d’application Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="e285a-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="e285a-116">Favoris gérés et raccourcis de page d’accueil</span><span class="sxs-lookup"><span data-stu-id="e285a-116">Managed favorites and home page shortcuts</span></span>
