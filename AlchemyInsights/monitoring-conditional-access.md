---
title: Surveillance de l’accès conditionnel
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468355"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="9536f-102">Surveillance de l’accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="9536f-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="9536f-p101">Les utilisateurs ciblés avec accès conditionnel reçoit un message électronique de notification si elles ne remplissent pas les conditions d’accès de votre organisation. Pour résoudre, nous vous recommandons d’une ou plusieurs des solutions suivantes :</span><span class="sxs-lookup"><span data-stu-id="9536f-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="9536f-p102">Si le périphérique est censé être inscrit, informer l’utilisateur à accéder à l’application de portail d’entreprise et vérifiez qu’il apparaît dans le portail d’entreprise. Le cas contraire, l’utilisateur doit s’inscrire l’appareil.</span><span class="sxs-lookup"><span data-stu-id="9536f-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="9536f-p103">Dans le portail Azure, accédez à **Intune \> conformité périphérique**. Sous **Moniteur** , cliquez sur **la conformité du périphérique**. Afficher l’état de conformité de périphérique pour vérifier que le périphérique de l’utilisateur est marqué comme conforme.</span><span class="sxs-lookup"><span data-stu-id="9536f-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="9536f-p104">Dans le portail Azure, accédez à **Intune \> conformité périphérique**. Sous **Gérer**, cliquez sur **stratégies**. Dans la liste des stratégies de conformité, vérifiez qu’un profil est attribué au périphérique de l’utilisateur. Si aucun profil n’est assigné, Intune ne sera pas en mesure de confirmer le statut de conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="9536f-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="9536f-114">Modifier l’affectation d’accès conditionnel de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9536f-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="9536f-115">Dans le portail Azure, accédez à **Intune \> accès conditionnel \> stratégies**</span><span class="sxs-lookup"><span data-stu-id="9536f-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="9536f-116">Sélectionnez une stratégie dans la liste</span><span class="sxs-lookup"><span data-stu-id="9536f-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="9536f-117">Cliquez sur **utilisateurs et groupes**</span><span class="sxs-lookup"><span data-stu-id="9536f-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="9536f-p105">Pour cibler une stratégie à une personne spécifique, ajoutez-les à la liste **d’inclusion** . Pour vous assurer qu’une personne est omise de la stratégie, les ajouter à la liste **à exclure** .</span><span class="sxs-lookup"><span data-stu-id="9536f-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="9536f-120">En savoir plus : [comment surveiller l’accès conditionnel périphériques](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="9536f-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

