---
title: Surveiller l’accès conditionnel à Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417109"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="9a0b8-102">Surveiller l’accès conditionnel à Intune</span><span class="sxs-lookup"><span data-stu-id="9a0b8-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="9a0b8-103">Les utilisateurs ciblés avec un accès conditionnel recevront un e-mail de notification s’ils ne répondent pas aux exigences d’accès de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9a0b8-104">Pour résoudre ce problème, nous vous recommandons d’apporter une ou plusieurs des solutions suivantes :</span><span class="sxs-lookup"><span data-stu-id="9a0b8-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="9a0b8-105">Si l’appareil est supposé être inscrit, conseillez à l’utilisateur d’utiliser l’application Portail d’entreprise et de vérifier qu’elle apparaît dans le portail d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9a0b8-106">Si ce n’est pas le cas, l’utilisateur doit inscrire l’appareil.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="9a0b8-107">Dans le portail Azure, allez à la conformité **des appareils Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="9a0b8-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="9a0b8-108">Pour afficher le rapport de conformité de votre appareil afin de vérifier que l’appareil de l’utilisateur est marqué comme conforme, sous **Surveiller,** cliquez sur **Conformité de l’appareil.**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="9a0b8-109">Dans le portail Azure, allez à la conformité **des appareils Intune.**  >  </span><span class="sxs-lookup"><span data-stu-id="9a0b8-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="9a0b8-110">Sous **Gérer, cliquez** sur **Stratégies.**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="9a0b8-111">Dans la liste des stratégies de conformité, vérifiez qu’un profil est affecté à l’appareil de votre utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9a0b8-112">Si aucun profil n’est affecté, Intune ne sera pas en mesure de confirmer l’état de conformité de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="9a0b8-113">Modifier l’affectation d’accès conditionnel de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="9a0b8-114">Dans le portail Azure, accédez à Stratégies d’accès conditionnel **Intune,** sélectionnez une stratégie dans la liste, puis cliquez sur Utilisateurs  >    >   **et groupes.**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="9a0b8-115">Pour cibler une stratégie à un autre, ajoutez-la à la **liste Inclure.**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="9a0b8-116">Pour vous assurer qu’une personne est omise de la stratégie, ajoutez-la à la **liste Exclure.**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="9a0b8-117">**Liens utiles :**</span><span class="sxs-lookup"><span data-stu-id="9a0b8-117">**Helpful links:**</span></span>

- [<span data-ttu-id="9a0b8-118">Vue d’ensemble de la conformité des appareils</span><span class="sxs-lookup"><span data-stu-id="9a0b8-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="9a0b8-119">Dépannage de l’ac</span><span class="sxs-lookup"><span data-stu-id="9a0b8-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="9a0b8-120">Stratégie de dépannage</span><span class="sxs-lookup"><span data-stu-id="9a0b8-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="9a0b8-121">Surveillance de la conformité des appareils Intune</span><span class="sxs-lookup"><span data-stu-id="9a0b8-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="9a0b8-122">Ces étapes sont utiles uniquement dans le dépannage de l’accès conditionnel à la fonctionnalité Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="9a0b8-123">Il est également possible de mettre en quarantaine un appareil qui bloque son accès à la messagerie avec la stratégie Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a0b8-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="9a0b8-124">Pour plus d’informations sur la gestion des appareils Exchange, voir [**ici.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="9a0b8-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
