---
title: Se connectez automatiquement à Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398727"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="4bc23-102">Se connectez automatiquement à Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="4bc23-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="4bc23-103">Microsoft Edge utilise le compte par défaut du système d’exploitation pour se connecter automatiquement à un utilisateur en fonction de la configuration de son appareil.</span><span class="sxs-lookup"><span data-stu-id="4bc23-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="4bc23-104">Les scénarios de chaque type de configuration d’appareil et de son processus de signature utilisateur dépendant sont décrits ci-dessous :</span><span class="sxs-lookup"><span data-stu-id="4bc23-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="4bc23-105">**L’appareil est hybride/AAD-J**: cette option est disponible sur Windows 10, Windows de bas niveau et les versions serveur correspondantes.</span><span class="sxs-lookup"><span data-stu-id="4bc23-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="4bc23-106">Les utilisateurs sont automatiquement signés avec leurs comptes Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="4bc23-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="4bc23-107">**L’appareil est joint au** domaine : cette option est disponible sur Windows 10, Windows de bas niveau et les versions de serveur correspondantes.</span><span class="sxs-lookup"><span data-stu-id="4bc23-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="4bc23-108">Par défaut, les utilisateurs ayant des comptes de domaine ne sont pas automatiquement signés ; pour activer la signature automatique pour eux, utilisez la **stratégie ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="4bc23-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="4bc23-109">Pour activer la connectez-vous automatique pour les utilisateurs ayant des comptes Azure AD, envisagez de rejoindre leurs appareils de façon hybride.</span><span class="sxs-lookup"><span data-stu-id="4bc23-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="4bc23-110">Le compte par défaut du système **d’exploitation** est un compte Microsoft : cette option est disponible sur Windows 10 RS3 (version 1709, build 10.0.16299) et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="4bc23-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="4bc23-111">Il est peu probable que le scénario se produise sur les appareils d’entreprise.</span><span class="sxs-lookup"><span data-stu-id="4bc23-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="4bc23-112">Toutefois, si le compte par défaut du système d’exploitation est un compte Microsoft, Microsoft Edge se connecte automatiquement à l’utilisateur avec le compte Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4bc23-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
