---
title: Une erreur de validation d'erreur de jeton d'accès s'est produite lors de l'embarquement d'Analyses du bureau
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813686"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="38afa-102">Erreur « Une erreur s'est produite lors de la validation du jeton d'accès » lors de l'intégration de Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="38afa-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="38afa-103">Cette erreur est normalement observée à l'expiration du jeton d'authentification.</span><span class="sxs-lookup"><span data-stu-id="38afa-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="38afa-104">En règle générale, l'actualisation de la page actualisé le jeton.</span><span class="sxs-lookup"><span data-stu-id="38afa-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="38afa-105">Toutefois, ce problème peut persister s'il existe des stratégies d'accès conditionnel appliquées au compte utilisé pour l'analyse du bureau à bord.</span><span class="sxs-lookup"><span data-stu-id="38afa-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="38afa-106">Vous pouvez consulter les journaux de connexion Azure AD dans le portail Azure pour voir s'il existe des échecs de connexion pour le compte utilisé pour l'intégration d'Analyses du bureau.</span><span class="sxs-lookup"><span data-stu-id="38afa-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="38afa-107">Pour plus d'informations sur l'accès conditionnel, voir [Planifier votre déploiement d'accès conditionnel.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="38afa-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>