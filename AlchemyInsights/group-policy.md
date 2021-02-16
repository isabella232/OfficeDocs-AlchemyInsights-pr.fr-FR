---
title: Stratégie de groupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243902"
---
# <a name="group-policy"></a><span data-ttu-id="cae3c-102">Stratégie de groupe</span><span class="sxs-lookup"><span data-stu-id="cae3c-102">Group policy</span></span>

<span data-ttu-id="cae3c-103">Les paramètres des objets utilisateur et ordinateur dans Azure Active Directory Domain Services (Azure AD DS) sont souvent gérés à l’aide d’objets de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="cae3c-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="cae3c-104">Azure AD DS inclut des objets de stratégie de groupe intégrés pour les utilisateurs AADDC et les conteneurs d’ordinateurs AADDC.</span><span class="sxs-lookup"><span data-stu-id="cae3c-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="cae3c-105">Vous pouvez personnaliser ces objets de stratégie de groupe intégrés pour configurer une stratégie de groupe selon les besoins de votre environnement.</span><span class="sxs-lookup"><span data-stu-id="cae3c-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="cae3c-106">Les membres du groupe d’administrateurs Azure AD DC ont des privilèges d’administration de stratégie de groupe dans le domaine Azure AD DS et peuvent également créer des objets de stratégies de groupe et des unités d’organisation personnalisées.</span><span class="sxs-lookup"><span data-stu-id="cae3c-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="cae3c-107">Pour plus d’informations sur la stratégie de groupe et son fonctionnement, consultez [Vue d’ensemble des stratégies de groupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="cae3c-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="cae3c-108">Dans un environnement hybride, les stratégies de groupe configurées dans un environnement AD DS local ne sont pas synchronisées avec Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="cae3c-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="cae3c-109">Pour définir les paramètres de configuration des utilisateurs ou des ordinateurs dans Azure AD DS, modifiez l’un des objectifs de groupe par défaut ou créez un groupe de travail personnalisé.</span><span class="sxs-lookup"><span data-stu-id="cae3c-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="cae3c-110">Cet article [Gérer des stratégie de groupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vous explique comment installer les outils de gestion des stratégies de groupe, comment modifier les objets de stratégie de groupe intégrés et comment créer des objets de stratégie de groupe personnalisés.</span><span class="sxs-lookup"><span data-stu-id="cae3c-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



