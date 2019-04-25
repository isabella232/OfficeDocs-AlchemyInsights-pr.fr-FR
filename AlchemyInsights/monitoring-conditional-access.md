---
title: Surveillance de l'accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418467"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="cb19c-102">Surveillance de l'accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="cb19c-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="cb19c-103">Les utilisateurs ciblés avec l'accès conditionnel recevront un courrier électronique de notification s'ils ne répondent pas aux exigences d'accès de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="cb19c-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="cb19c-104">Pour résoudre ce qui suit, nous vous recommandons d'utiliser une ou plusieurs des solutions suivantes:</span><span class="sxs-lookup"><span data-stu-id="cb19c-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="cb19c-105">Si le périphérique est présumé être inscrire, conseillez-lui d'accéder à l'application portail d'entreprise et de vérifier qu'il apparaît dans le portail d'entreprise.</span><span class="sxs-lookup"><span data-stu-id="cb19c-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="cb19c-106">Si ce n'est pas le cas, l'utilisateur doit inscrire l'appareil.</span><span class="sxs-lookup"><span data-stu-id="cb19c-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="cb19c-107">Dans le portail Azure, accédez **à \> Intune Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="cb19c-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="cb19c-108">Sous **analyse** , cliquez sur **conformité des appareils**.</span><span class="sxs-lookup"><span data-stu-id="cb19c-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="cb19c-109">Affichez votre rapport de conformité des appareils pour vérifier que l'appareil de l'utilisateur est marqué comme étant compatible.</span><span class="sxs-lookup"><span data-stu-id="cb19c-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="cb19c-110">Dans le portail Azure, accédez **à \> Intune Device Compliance**.</span><span class="sxs-lookup"><span data-stu-id="cb19c-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="cb19c-111">Sous **gérer**, cliquez sur **stratégies**.</span><span class="sxs-lookup"><span data-stu-id="cb19c-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="cb19c-112">Dans la liste des stratégies de conformité, vérifiez qu'un profil est affecté à l'appareil de votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cb19c-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="cb19c-113">Si aucun profil n'est affecté, Intune ne pourra pas confirmer l'état de conformité de l'appareil.</span><span class="sxs-lookup"><span data-stu-id="cb19c-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="cb19c-114">Modifiez l'attribution d'accès conditionnel de l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cb19c-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="cb19c-115">Dans le portail Azure, accéder **aux \> stratégies d' \> accès conditionnel Intune**</span><span class="sxs-lookup"><span data-stu-id="cb19c-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="cb19c-116">Sélectionner une stratégie dans la liste</span><span class="sxs-lookup"><span data-stu-id="cb19c-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="cb19c-117">Cliquez sur **utilisateurs et groupes**</span><span class="sxs-lookup"><span data-stu-id="cb19c-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="cb19c-118">Pour cibler une stratégie spécifique à une personne, ajoutez-la à la liste **inclure** .</span><span class="sxs-lookup"><span data-stu-id="cb19c-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="cb19c-119">Pour vous assurer qu'une personne est omise de la stratégie, ajoutez-la à la liste d' **exclusion** .</span><span class="sxs-lookup"><span data-stu-id="cb19c-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="cb19c-120">En savoir plus: [comment surveiller les appareils d'accès conditionnel](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="cb19c-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

