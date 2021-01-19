---
title: Problèmes de consentement de l’administrateur
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888300"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="6fd08-102">Problèmes de consentement de l’administrateur</span><span class="sxs-lookup"><span data-stu-id="6fd08-102">Admin consent issues</span></span>

1. <span data-ttu-id="6fd08-103">Activez le [flux de travail de consentement de](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) l’administrateur pour permettre aux utilisateurs de demander l’approbation de l’administrateur directement à partir de l’écran de consentement.</span><span class="sxs-lookup"><span data-stu-id="6fd08-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="6fd08-104">Si vous ou les utilisateurs de votre application constatez des erreurs inattendues pendant le processus de consentement, consultez cet article pour les étapes de résolution des problèmes : [Erreur](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)inattendue lors de l’application du consentement.</span><span class="sxs-lookup"><span data-stu-id="6fd08-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="6fd08-105">En savoir plus sur le consentement de [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) l’administrateur sur la plateforme d’identité [Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)sur le fonctionnement de l’invite de consentement et sur l’évaluation d’une demande de consentement d’administrateur à l’échelle [du client.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="6fd08-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="6fd08-106">Les applications qui s’intègrent à la plateforme d’identités Microsoft suivent un modèle d’autorisation qui permet aux utilisateurs et aux administrateurs de contrôler la façon dont les données sont accessibles.</span><span class="sxs-lookup"><span data-stu-id="6fd08-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6fd08-107">L’implémentation du modèle d’autorisation a été mise à jour sur le point de terminaison de la plateforme d’identités Microsoft et elle modifie la façon dont une application doit interagir avec la plateforme d’identités Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6fd08-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6fd08-108">Voir [autorisations et consentement](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) dans le point de terminaison de la plateforme d’identités Microsoft pour obtenir une vue d’ensemble de ce modèle d’autorisation, y compris les étendues, les autorisations et le consentement.</span><span class="sxs-lookup"><span data-stu-id="6fd08-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>