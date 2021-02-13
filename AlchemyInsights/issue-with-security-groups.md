---
title: Problème lié aux groupes de sécurité
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162924"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="0efcd-102">Problème lié aux groupes de sécurité</span><span class="sxs-lookup"><span data-stu-id="0efcd-102">Issue with security groups</span></span>

<span data-ttu-id="0efcd-103">**Si vous obtenez l’erreur réseau AADDS104**</span><span class="sxs-lookup"><span data-stu-id="0efcd-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="0efcd-104">Les règles de groupe de sécurité réseau non valides constituent la cause la plus fréquente d’erreurs réseau pour Azure Active Directory Domain Services (AD DS).</span><span class="sxs-lookup"><span data-stu-id="0efcd-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="0efcd-105">Le groupe de sécurité réseau du réseau virtuel doit autoriser l’accès à des ports et à des protocoles spécifiques.</span><span class="sxs-lookup"><span data-stu-id="0efcd-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="0efcd-106">Si le groupe de sécurité bloque l’accès à ces ports, la plateforme Azure ne peut pas surveiller, ni mettre à jour le domaine géré.</span><span class="sxs-lookup"><span data-stu-id="0efcd-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="0efcd-107">Cela a également un impact sur la synchronisation entre Azure AD et Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0efcd-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="0efcd-108">Veillez à laisser les ports par défaut ouverts pour éviter une interruption du service.</span><span class="sxs-lookup"><span data-stu-id="0efcd-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="0efcd-109">Si vous souhaitez en savoir plus sur les alertes courantes correspondant aux problèmes de configuration des groupes de sécurité réseau, veuillez consulter la rubrique [Ajouter et vérifier des groupes de sécurité](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="0efcd-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
