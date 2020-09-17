---
title: Une erreur s’est produite lors de la validation de l’erreur de jeton d’accès lors de l’intégration de l’analyse de bureau
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783549"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="00784-102">Erreur « une erreur de validation du jeton d’accès » s’est produite lors de l’intégration de l’analyse de bureau</span><span class="sxs-lookup"><span data-stu-id="00784-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="00784-103">Cette erreur est normalement observée lorsque le jeton d’authentification arrive à expiration.</span><span class="sxs-lookup"><span data-stu-id="00784-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="00784-104">En règle générale, l’actualisation de la page actualise le jeton.</span><span class="sxs-lookup"><span data-stu-id="00784-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="00784-105">Toutefois, ce problème peut persister si des stratégies d’accès conditionnel sont appliquées au compte utilisé pour l’analyse de bureau intégrée.</span><span class="sxs-lookup"><span data-stu-id="00784-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="00784-106">Vous pouvez consulter les journaux de connexion Azure AD dans le portail Azure pour voir s’il existe des échecs de connexion pour le compte utilisé pour l’intégration de l’analyse de bureau.</span><span class="sxs-lookup"><span data-stu-id="00784-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="00784-107">Pour plus d’informations sur l’accès conditionnel, consultez [la rubrique planifier votre déploiement d’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="00784-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>