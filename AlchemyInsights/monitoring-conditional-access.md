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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708672"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="3b4e2-102">Surveillance de l’accès conditionnel pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3b4e2-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="3b4e2-103">Les utilisateurs ciblés avec un accès conditionnel recevront un e-mail de notification s’ils ne répondent pas aux exigences d’accès de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="3b4e2-104">Pour résoudre ce problème, nous vous recommandons d’apporter une ou plusieurs des solutions suivantes :</span><span class="sxs-lookup"><span data-stu-id="3b4e2-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="3b4e2-105">Si l’appareil est supposé être inscrit, conseillez à l’utilisateur d’utiliser l’application Portail d’entreprise et de vérifier qu’elle apparaît dans le portail d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="3b4e2-106">Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="3b4e2-107">Dans le portail Azure, allez sur Intune > conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="3b4e2-108">Sous Surveiller, cliquez sur Conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="3b4e2-109">Affichez le rapport de conformité de votre appareil pour vérifier que l’appareil de l’utilisateur est marqué comme conforme.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="3b4e2-110">Dans le portail Azure, allez sur Intune > conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="3b4e2-111">Sous Gérer, cliquez sur Stratégies.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-111">Under Manage, click Policies.</span></span> <span data-ttu-id="3b4e2-112">Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="3b4e2-113">Si aucun profil n’est affecté, Intune ne sera pas en mesure de confirmer l’état de conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="3b4e2-114">Modifiez l’affectation d’accès conditionnel de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="3b4e2-115">Dans le portail Azure, accédez à **Stratégies d’accès**  >  **conditionnel** Intune.  >  </span><span class="sxs-lookup"><span data-stu-id="3b4e2-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="3b4e2-116">Sélectionnez une stratégie dans la liste.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="3b4e2-117">Cliquez sur Utilisateurs et groupes.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-117">Click Users and groups.</span></span>
4. <span data-ttu-id="3b4e2-118">Pour cibler une stratégie à une personne, ajoutez-la à la liste Inclure.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="3b4e2-119">Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la liste Exclure.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="3b4e2-120">Liens utiles :</span><span class="sxs-lookup"><span data-stu-id="3b4e2-120">Helpful links:</span></span>

[<span data-ttu-id="3b4e2-121">Vue d’ensemble de la conformité des appareils</span><span class="sxs-lookup"><span data-stu-id="3b4e2-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="3b4e2-122">Dépannage de l’ac</span><span class="sxs-lookup"><span data-stu-id="3b4e2-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3b4e2-123">Stratégie de dépannage</span><span class="sxs-lookup"><span data-stu-id="3b4e2-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="3b4e2-124">Surveillance de la conformité des appareils Intune</span><span class="sxs-lookup"><span data-stu-id="3b4e2-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="3b4e2-125">Remarque : ces étapes sont uniquement utiles pour résoudre les problèmes d’accès conditionnel à la fonctionnalité Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="3b4e2-126">Il est également possible de mettre en quarantaine un appareil qui bloque son accès à la messagerie avec la stratégie Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b4e2-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="3b4e2-127">Pour plus d’informations sur la gestion des appareils Exchange, voir [ici]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="3b4e2-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
