---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704784"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="fcc8b-102">Accès conditionnel avec Intune</span><span class="sxs-lookup"><span data-stu-id="fcc8b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="fcc8b-103">**L’utilisation de l’accès** conditionnel avec Intune nécessite 3 étapes :</span><span class="sxs-lookup"><span data-stu-id="fcc8b-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="fcc8b-104">Créez  **une stratégie de**  conformité ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) pour définir les paramètres qui doivent être respectés avant que l’appareil soit considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="fcc8b-105">Par exemple, un appareil doit avoir une broche d’au moins 6 chiffres avant d’être considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="fcc8b-106">Créez **une stratégie d’accès**  conditionnel qui définit les ressources protégées et les conditions qui doivent être remplies pour accéder à ces ressources.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="fcc8b-107">[Par exemple, un](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  appareil doit être conforme avant d’accéder à la messagerie d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="fcc8b-108">Assurez-vous **que les stratégies de**  conformité et les  **stratégies**  d’accès conditionnel sont ciblées sur les groupes d’utilisateurs souhaités.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="fcc8b-109">Cela peut nécessiter la création de groupes spécifiques d’utilisateurs dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fcc8b-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="fcc8b-110">**Liens utiles :**</span><span class="sxs-lookup"><span data-stu-id="fcc8b-110">**Helpful links:**</span></span>

[<span data-ttu-id="fcc8b-111">Vue d’ensemble de la conformité des appareils</span><span class="sxs-lookup"><span data-stu-id="fcc8b-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="fcc8b-112">Dépannage de l’ac</span><span class="sxs-lookup"><span data-stu-id="fcc8b-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="fcc8b-113">Stratégie de dépannage</span><span class="sxs-lookup"><span data-stu-id="fcc8b-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="fcc8b-114">Pour protéger la messagerie électronique (Exchange Online) contre l’accès par des appareils non conformes, les deux documents doivent être suivis :</span><span class="sxs-lookup"><span data-stu-id="fcc8b-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="fcc8b-115">Protéger l’accès à la messagerie à partir d’appareils à l’aide d’EAS</span><span class="sxs-lookup"><span data-stu-id="fcc8b-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="fcc8b-116">Protéger l’accès à la messagerie à partir d’appareils utilisant des clients d’authentification modernes tels qu’Outlook</span><span class="sxs-lookup"><span data-stu-id="fcc8b-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)