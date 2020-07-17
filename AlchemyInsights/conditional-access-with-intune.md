---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931428"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="436a7-102">Accès conditionnel avec Intune</span><span class="sxs-lookup"><span data-stu-id="436a7-102">Conditional Access with Intune</span></span>

<span data-ttu-id="436a7-103">L’utilisation de l' **accès conditionnel** avec Intune nécessite 3 étapes :</span><span class="sxs-lookup"><span data-stu-id="436a7-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="436a7-104">Créez une **stratégie de conformité** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pour définir les paramètres qui doivent être satisfaits pour que l’appareil soit considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="436a7-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="436a7-105">Par exemple, un appareil doit avoir un code confidentiel d’au moins 6 chiffres avant d’être considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="436a7-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="436a7-106">Créer une **stratégie d’accès conditionnel** qui définit les ressources à protéger et les conditions à respecter pour accéder à ces ressources.</span><span class="sxs-lookup"><span data-stu-id="436a7-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="436a7-107">[Par exemple,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) un appareil doit être conforme avant d’accéder à la messagerie d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="436a7-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="436a7-108">Assurez-vous que les stratégies de **conformité** et les **stratégies d’accès conditionnel** sont ciblées pour les groupes d’utilisateurs souhaités.</span><span class="sxs-lookup"><span data-stu-id="436a7-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="436a7-109">Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="436a7-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="436a7-110">**Liens utiles :**</span><span class="sxs-lookup"><span data-stu-id="436a7-110">**Helpful links:**</span></span>

[<span data-ttu-id="436a7-111">Présentation de la conformité des appareils</span><span class="sxs-lookup"><span data-stu-id="436a7-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="436a7-112">Dépannage de l’autorité de certification</span><span class="sxs-lookup"><span data-stu-id="436a7-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="436a7-113">Stratégie de résolution des problèmes</span><span class="sxs-lookup"><span data-stu-id="436a7-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="436a7-114">Pour protéger les messages électroniques (Exchange Online) contre les accès par des appareils non conformes, les deux documents doivent être suivis :</span><span class="sxs-lookup"><span data-stu-id="436a7-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="436a7-115">Protection de l’accès au courrier électronique à partir d’appareils utilisant EAS</span><span class="sxs-lookup"><span data-stu-id="436a7-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="436a7-116">Protéger l’accès à la messagerie des appareils utilisant des clients d’authentification modernes comme Outlook</span><span class="sxs-lookup"><span data-stu-id="436a7-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)