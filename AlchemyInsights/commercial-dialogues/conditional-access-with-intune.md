---
title: Utilisation de l’accès conditionnel avec Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736771"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="cdeaa-102">Utilisation de l’accès conditionnel avec Intune</span><span class="sxs-lookup"><span data-stu-id="cdeaa-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="cdeaa-103">L’utilisation de l’accès conditionnel avec Intune nécessite 3 étapes :</span><span class="sxs-lookup"><span data-stu-id="cdeaa-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="cdeaa-104">Créez une stratégie de conformité pour définir des paramètres qui doivent être respectés avant que l’appareil soit considéré comme conforme. Par exemple, un appareil doit avoir une broche d’au moins 6 chiffres avant d’être considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="cdeaa-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="cdeaa-105">Créez une stratégie d’accès conditionnel qui définit les ressources protégées et les conditions qui doivent être remplies pour accéder à ces ressources. Par exemple, un appareil doit être conforme avant d’accéder à la messagerie d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="cdeaa-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="cdeaa-106">Assurez-vous que les stratégies de conformité et les stratégies d’accès conditionnel sont ciblées sur les groupes d’utilisateurs souhaités. Cela peut nécessiter la création de groupes spécifiques d’utilisateurs dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cdeaa-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="cdeaa-107">En savoir plus</span><span class="sxs-lookup"><span data-stu-id="cdeaa-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
