---
title: Accès conditionnel avec Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36504992"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8bec3-102">Accès conditionnel avec Intune</span><span class="sxs-lookup"><span data-stu-id="8bec3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8bec3-103">L’utilisation de l' **accès conditionnel** avec Intune nécessite 3 étapes :</span><span class="sxs-lookup"><span data-stu-id="8bec3-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="8bec3-104">Créer une **stratégie d’accès conditionnel** qui définit les ressources à protéger et les conditions à respecter pour accéder à ces ressources.</span><span class="sxs-lookup"><span data-stu-id="8bec3-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="8bec3-105">Par exemple, un appareil doit être conforme avant d’accéder à la messagerie d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="8bec3-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="8bec3-106">Créez une **stratégie de conformité** pour définir les paramètres qui doivent être satisfaits pour que l’appareil soit considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="8bec3-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="8bec3-107">Par exemple, un appareil doit avoir un code confidentiel d’au moins 6 chiffres avant d’être considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="8bec3-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="8bec3-108">S’assurer que les stratégies de **conformité** et les **stratégies d’accès conditionnel** sont ciblées pour les groupes d’utilisateurs souhaités.</span><span class="sxs-lookup"><span data-stu-id="8bec3-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="8bec3-109">Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8bec3-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="8bec3-110">En savoir plus :</span><span class="sxs-lookup"><span data-stu-id="8bec3-110">Read more:</span></span>
  
- [<span data-ttu-id="8bec3-111">Meilleures pratiques en matière d’accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="8bec3-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="8bec3-112">Prise en main de l’accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="8bec3-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

