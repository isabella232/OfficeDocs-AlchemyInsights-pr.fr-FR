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
# <a name="grant-permissions"></a>Accorder des autorisations

1. Octroi du consentement de l’administrateur à l’échelle du client : voir accorder le consentement de l’administrateur à l’échelle du client à une [application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) pour obtenir des instructions détaillées sur l’octroi du consentement d’administrateur à l’échelle du client à partir du portail Azure, à l’aide d’Azure AD PowerShell ou de l’invite de consentement elle-même.
1. Octroi du **consentement** pour le compte d’un utilisateur spécifique : au lieu d’accorder le consentement à l’ensemble de l’organisation, un administrateur peut également utiliser l’API [Microsoft Graph](https://docs.microsoft.com/graph/use-the-api) pour accorder le consentement aux autorisations déléguées pour le compte d’un utilisateur unique. Pour plus d’informations, [voir Obtenir l’accès au nom d’un utilisateur.](https://docs.microsoft.com/graph/auth-v2-user)