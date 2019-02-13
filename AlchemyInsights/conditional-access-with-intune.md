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
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935930"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="83b67-102">Accès conditionnel avec Intune</span><span class="sxs-lookup"><span data-stu-id="83b67-102">Conditional Access with Intune</span></span>

<span data-ttu-id="83b67-103">À l’aide de **L’accès conditionnel** avec Intune requiert 3 comme suit :</span><span class="sxs-lookup"><span data-stu-id="83b67-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="83b67-p101">Créer une **Stratégie d’accès conditionnel** qui définit les ressources qui sont protégés, et les conditions qui doivent être remplies pour accéder à ces ressources. Par exemple, un périphérique doit être conforme avant d’accéder à la messagerie d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="83b67-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="83b67-p102">Créer une **Stratégie de conformité** pour définir les paramètres qui doivent être remplis avant que le périphérique est considéré comme conforme. Par exemple, un périphérique doit avoir un code confidentiel d’au moins 6 chiffres est considéré comme conforme.</span><span class="sxs-lookup"><span data-stu-id="83b67-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="83b67-p103">Vérifier les **Stratégies de conformité** et **Les stratégies d’accès conditionnel** destinées à des groupes d’utilisateurs requis. Cela peut nécessiter la création de groupes d’utilisateurs spécifiques dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83b67-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="83b67-110">En savoir plus :</span><span class="sxs-lookup"><span data-stu-id="83b67-110">Read more:</span></span>
  
- [<span data-ttu-id="83b67-111">Meilleures pratiques en matière de conditionnelle accès</span><span class="sxs-lookup"><span data-stu-id="83b67-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="83b67-112">Mise en route avec accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="83b67-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

