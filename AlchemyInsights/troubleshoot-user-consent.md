---
title: Résoudre les problèmes de consentement de l’utilisateur
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897722"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="b6aad-102">Résoudre les problèmes de consentement de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="b6aad-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="b6aad-103">Vous pouvez configurer la façon dont les utilisateurs finaux consentent aux applications via le portail Azure ou PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b6aad-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="b6aad-104">Pour plus [d’informations, voir paramètres](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) de consentement utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b6aad-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="b6aad-105">Un administrateur peut également utiliser [l’API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) pour accorder le consentement à des autorisations déléguées au nom d’un seul utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b6aad-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="b6aad-106">Pour plus d’informations, [voir Obtenir l’accès au nom d’un utilisateur.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="b6aad-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="b6aad-107">[Erreurs de consentement de](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)l’utilisateur : cet article traite des erreurs qui peuvent se produire pendant le processus de consentement à une application.</span><span class="sxs-lookup"><span data-stu-id="b6aad-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="b6aad-108">Si vous dépannagez des invites de consentement inattendues qui ne contiennent aucun message d’erreur, consultez Scénarios d’authentification [pour Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="b6aad-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>