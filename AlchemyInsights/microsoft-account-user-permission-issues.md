---
title: Résoudre le problème-utilisateur introuvable dans l’annuaire
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249911"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="eaa3d-102">Résoudre le problème-utilisateur introuvable dans l’annuaire</span><span class="sxs-lookup"><span data-stu-id="eaa3d-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="eaa3d-103">Si les utilisateurs reçoivent un message d’erreur indiquant que l’utilisateur est introuvable dans l’annuaire.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="eaa3d-104">Réessayez là où le type de problème est utilisateur non dans le répertoire.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="eaa3d-105">Vous pouvez effectuer les étapes suivantes pour résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="eaa3d-106">Assurez-vous que le compte qui a accepté l’invitation électronique est le même compte que celui utilisé pour la connexion ultérieure.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="eaa3d-107">Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="eaa3d-108">Pour plus d’informations, reportez-vous à la rubrique [gestion</a> des alias de votre compte Microsoft pour gérer la connexion à Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="eaa3d-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="eaa3d-109">Accédez à chaque site (s) dans lequel l’utilisateur reçoit l’erreur.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="eaa3d-110">Ajoutez «/_layouts/15/People.aspx/MembershipGroupId = 0» (dans les guillemets doubles) à la fin de l’URL du site.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="eaa3d-111">Exemple: https://< «contoso» >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="eaa3d-112">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-112">Select the user from the list.</span></span>

- <span data-ttu-id="eaa3d-113">Cliquez sur **Supprimer les autorisations des utilisateurs** du ruban.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="eaa3d-114">Rajoutez l’utilisateur et renvoyez-le à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="eaa3d-114">Add back the User and Resend the invite to the user.</span></span>

