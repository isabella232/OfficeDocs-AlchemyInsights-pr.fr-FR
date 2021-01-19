---
title: Accorder des autorisations
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897719"
---
# <a name="grant-permissions"></a><span data-ttu-id="12b6d-102">Accorder des autorisations</span><span class="sxs-lookup"><span data-stu-id="12b6d-102">Grant permissions</span></span>

1. <span data-ttu-id="12b6d-103">Octroi du consentement de l’administrateur à l’échelle du client : voir accorder le consentement de l’administrateur à l’échelle du client à une [application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) pour obtenir des instructions détaillées sur l’octroi du consentement d’administrateur à l’échelle du client à partir du portail Azure, à l’aide d’Azure AD PowerShell ou de l’invite de consentement elle-même.</span><span class="sxs-lookup"><span data-stu-id="12b6d-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="12b6d-104">Octroi du **consentement** pour le compte d’un utilisateur spécifique : au lieu d’accorder le consentement à l’ensemble de l’organisation, un administrateur peut également utiliser l’API [Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) pour accorder le consentement aux autorisations déléguées pour le compte d’un utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="12b6d-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="12b6d-105">Pour plus d’informations, [voir Obtenir l’accès au nom d’un utilisateur.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="12b6d-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>