---
title: Complément Teams pour Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617068"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="8cd08-102">Complément Teams pour Mac</span><span class="sxs-lookup"><span data-stu-id="8cd08-102">Teams add-in for Mac</span></span>

<span data-ttu-id="8cd08-103">Pour résoudre les problèmes liés à l’absence d’un complément Teams pour Mac, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="8cd08-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="8cd08-104">**Étape 1 :** si vous avez un environnement Exchange hybride (2016 CU3 ou version ultérieure requise), utilisez l’outil Test-HMA.ps1 pour confirmer que l’authentification moderne hybride est correctement configurée.</span><span class="sxs-lookup"><span data-stu-id="8cd08-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="8cd08-105">Pour plus d’informations, consultez [Validation de la configuration de l’authentification moderne hybride pour Outlook pour iOS et Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="8cd08-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="8cd08-106">**Remarque** utiliser le format d’adresse UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)), et non domaine\nomutilisateur.</span><span class="sxs-lookup"><span data-stu-id="8cd08-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="8cd08-107">Pour ce faire, même pour les utilisateurs disposant de boîtes aux lettres Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8cd08-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="8cd08-108">**Étape 2 :** demander à l’utilisateur d’accéder à **outils** > **Comptes**... dans Outlook pour Mac, recherchez et sélectionnez le compte.</span><span class="sxs-lookup"><span data-stu-id="8cd08-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="8cd08-109">Vérifiez que le nom d’utilisateur indiqué est au format UPN (par exemple, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="8cd08-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="8cd08-110">**Étape 3 :** confirmer que l’utilisateur est titulaire d’une licence Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8cd08-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="8cd08-111">L’utilisateur doit utiliser l’abonnement Office 365 pour Mac, le produit 16.24 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="8cd08-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>