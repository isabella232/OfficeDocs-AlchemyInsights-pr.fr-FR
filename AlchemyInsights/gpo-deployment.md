---
title: Déploiement d’un GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417012"
---
# <a name="gpo-deployment"></a><span data-ttu-id="e1d16-102">Déploiement d’un GPO</span><span class="sxs-lookup"><span data-stu-id="e1d16-102">GPO Deployment</span></span>

<span data-ttu-id="e1d16-103">Les paramètres des objets utilisateur et ordinateur dans Azure Active Directory Domain Services (Azure AD DS) sont souvent gérés à l’aide d’objets de stratégie de groupe.</span><span class="sxs-lookup"><span data-stu-id="e1d16-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="e1d16-104">Azure AD DS inclut des objets de stratégie de groupe intégrés pour les utilisateurs AADDC et les conteneurs d’ordinateurs AADDC.</span><span class="sxs-lookup"><span data-stu-id="e1d16-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="e1d16-105">Vous pouvez personnaliser ces objets de stratégie de groupe intégrés pour configurer une stratégie de groupe selon les besoins de votre environnement.</span><span class="sxs-lookup"><span data-stu-id="e1d16-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="e1d16-106">Les membres du groupe d’administrateurs Azure AD DC ont des privilèges d’administration de stratégie de groupe dans le domaine Azure AD DS et peuvent également créer des objets de stratégies de groupe et des unités d’organisation personnalisées.</span><span class="sxs-lookup"><span data-stu-id="e1d16-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="e1d16-107">Pour plus d’informations sur la stratégie de groupe et son fonctionnement, voir [Vue d’ensemble de la stratégie de groupe.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="e1d16-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="e1d16-108">Dans un environnement hybride, les stratégies de groupe configurées dans un environnement AD DS local ne sont pas synchronisées avec Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="e1d16-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="e1d16-109">Pour définir les paramètres de configuration des utilisateurs ou des ordinateurs dans Azure AD DS, modifiez l’un des objectifs de groupe par défaut ou créez un groupe de travail personnalisé.</span><span class="sxs-lookup"><span data-stu-id="e1d16-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="e1d16-110">Cet article [Gérer des stratégie de groupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vous explique comment installer les outils de gestion des stratégies de groupe, comment modifier les objets de stratégie de groupe intégrés et comment créer des objets de stratégie de groupe personnalisés.</span><span class="sxs-lookup"><span data-stu-id="e1d16-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
