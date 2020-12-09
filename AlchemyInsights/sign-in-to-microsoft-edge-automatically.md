---
title: Se connecter automatiquement à Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599467"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="ea2e4-102">Se connecter automatiquement à Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="ea2e4-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="ea2e4-103">Microsoft Edge utilise le compte par défaut du système d’exploitation pour se connecter automatiquement à un utilisateur en fonction de la configuration de l’appareil de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="ea2e4-104">Les scénarios de chaque type de configuration d’appareil et de processus de connexion de l’utilisateur dépendant sont décrits ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="ea2e4-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="ea2e4-105">**L’appareil est hybride/AAD-J**: cette option est disponible sur Windows 10, des fenêtres de bas niveau et des versions de serveur correspondantes.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ea2e4-106">Les utilisateurs sont automatiquement connectés avec leurs comptes Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="ea2e4-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="ea2e4-107">**L’appareil est joint à un domaine**: cette option est disponible dans Windows 10, les fenêtres de bas niveau et les versions de serveur correspondantes.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="ea2e4-108">Par défaut, les utilisateurs disposant de comptes de domaine ne sont pas connectés automatiquement ; pour activer la connexion automatique, utilisez la stratégie **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="ea2e4-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="ea2e4-109">Pour activer la connexion automatique pour les utilisateurs disposant de comptes Azure AD, envisagez la jonction hybride de leurs appareils.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="ea2e4-110">**Le compte par défaut du se est un compte Microsoft**: cette option est disponible sur Windows 10 RS3 (version 1709, Build 10.0.16299) et les versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="ea2e4-111">Il est peu probable que le scénario se produise sur les appareils de l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="ea2e4-112">Toutefois, si le compte par défaut du système d’exploitation est un compte Microsoft, Microsoft Edge se connectera automatiquement à l’utilisateur avec le compte Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ea2e4-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
