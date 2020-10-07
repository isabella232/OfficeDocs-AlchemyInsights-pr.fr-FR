---
title: Surveillance de l’accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366426"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="293ce-102">Surveillance de l’accès conditionnel pour Exchange</span><span class="sxs-lookup"><span data-stu-id="293ce-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="293ce-103">Les utilisateurs ciblés avec l’accès conditionnel recevront un courrier électronique de notification s’ils ne répondent pas aux exigences d’accès de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="293ce-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="293ce-104">Pour résoudre ce qui suit, nous vous recommandons d’utiliser une ou plusieurs des solutions suivantes :</span><span class="sxs-lookup"><span data-stu-id="293ce-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="293ce-105">Si le périphérique est présumé être inscrire, conseillez-lui d’accéder à l’application portail d’entreprise et de vérifier qu’il apparaît dans le portail d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="293ce-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="293ce-106">Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.</span><span class="sxs-lookup"><span data-stu-id="293ce-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="293ce-107">Dans le portail Azure, accédez à Intune > la conformité des appareils.</span><span class="sxs-lookup"><span data-stu-id="293ce-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="293ce-108">Sous analyse, cliquez sur conformité des appareils.</span><span class="sxs-lookup"><span data-stu-id="293ce-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="293ce-109">Affichez votre rapport de conformité des appareils pour vérifier que l’appareil de l’utilisateur est marqué comme étant compatible.</span><span class="sxs-lookup"><span data-stu-id="293ce-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="293ce-110">Dans le portail Azure, accédez à Intune > la conformité des appareils.</span><span class="sxs-lookup"><span data-stu-id="293ce-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="293ce-111">Sous gérer, cliquez sur stratégies.</span><span class="sxs-lookup"><span data-stu-id="293ce-111">Under Manage, click Policies.</span></span> <span data-ttu-id="293ce-112">Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="293ce-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="293ce-113">Si aucun profil n’est affecté, Intune ne pourra pas confirmer l’état de conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="293ce-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="293ce-114">Modifiez l’attribution d’accès conditionnel de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="293ce-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="293ce-115">Dans le portail Azure, accédez **Intune**aux stratégies d'  >  **accès conditionnel**Intune  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="293ce-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="293ce-116">Sélectionnez une stratégie dans la liste.</span><span class="sxs-lookup"><span data-stu-id="293ce-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="293ce-117">Cliquez sur utilisateurs et groupes.</span><span class="sxs-lookup"><span data-stu-id="293ce-117">Click Users and groups.</span></span>
4. <span data-ttu-id="293ce-118">Pour cibler une stratégie spécifique à une personne, ajoutez-la à la liste inclure.</span><span class="sxs-lookup"><span data-stu-id="293ce-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="293ce-119">Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la liste d’exclusion.</span><span class="sxs-lookup"><span data-stu-id="293ce-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="293ce-120">Liens utiles :</span><span class="sxs-lookup"><span data-stu-id="293ce-120">Helpful links:</span></span>

[<span data-ttu-id="293ce-121">Présentation de la conformité des appareils</span><span class="sxs-lookup"><span data-stu-id="293ce-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="293ce-122">Dépannage de l’autorité de certification</span><span class="sxs-lookup"><span data-stu-id="293ce-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="293ce-123">Stratégie de résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="293ce-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="293ce-124">Surveillance de la conformité des appareils Intune</span><span class="sxs-lookup"><span data-stu-id="293ce-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="293ce-125">Remarque : ces étapes ne sont utiles que pour résoudre les problèmes liés à l’accès conditionnel à la fonctionnalité Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="293ce-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="293ce-126">Il est également possible de mettre en quarantaine un appareil qui bloque l’accès à la messagerie avec la stratégie Exchange.</span><span class="sxs-lookup"><span data-stu-id="293ce-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="293ce-127">Vous trouverez plus d’informations sur la gestion des appareils Exchange [ici](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="293ce-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
