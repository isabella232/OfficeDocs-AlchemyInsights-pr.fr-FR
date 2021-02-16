---
title: Synchronisation des groupes
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
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243905"
---
# <a name="group-sync"></a><span data-ttu-id="7e988-102">Synchronisation des groupes</span><span class="sxs-lookup"><span data-stu-id="7e988-102">Group sync</span></span>

<span data-ttu-id="7e988-103">Cet article fournit des conseils sur la synchronisation des groupes.</span><span class="sxs-lookup"><span data-stu-id="7e988-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="7e988-104">Si un administrateur général ou propriétaire de groupe n’est pas en mesure de modifier les propriétés du groupe ou d’ajouter des membres ou d’attribuer des propriétaires dans le Portail Microsoft Azure, assurez-vous que la source de l’autorité pour le groupe est Azure Active Directory (Azure AD) pour l’administrateur général ou le propriétaire du groupe afin de modifier le groupe.</span><span class="sxs-lookup"><span data-stu-id="7e988-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="7e988-105">Avant d’essayer de supprimer un groupe synchronisé dans Azure AD, assurez-vous que vous avez [supprimé toutes les licences attribuées](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) pour éviter les erreurs.</span><span class="sxs-lookup"><span data-stu-id="7e988-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="7e988-106">Pour comprendre comment synchroniser les utilisateurs, les groupes et les contacts, consultez [Synchronisation d’Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), et suivez [Synchronisation d’un groupe local sur Azure à l’aide d’Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) pour synchroniser des groupes locaux à l’aide de Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7e988-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="7e988-107">Suivez ce guide [Erreurs de résolution des problèmes pendant la synchronisation](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) pour résoudre des problèmes d’erreurs courantes lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="7e988-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

