---
title: Résoudre le problème-utilisateur introuvable dans l’annuaire
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702736"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="33d94-102">Résoudre le problème-utilisateur introuvable dans l’annuaire</span><span class="sxs-lookup"><span data-stu-id="33d94-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="33d94-103">Si les utilisateurs reçoivent un message d’erreur indiquant que l’utilisateur est introuvable dans le répertoire, réessayez en indiquant que le type de problème est User not in Directory.</span><span class="sxs-lookup"><span data-stu-id="33d94-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="33d94-104">Vous pouvez effectuer les étapes suivantes pour résoudre le problème.</span><span class="sxs-lookup"><span data-stu-id="33d94-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="33d94-105">Assurez-vous que le compte qui a accepté l’invitation électronique est le même compte que celui utilisé pour la connexion ultérieure.</span><span class="sxs-lookup"><span data-stu-id="33d94-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="33d94-106">Assurez-vous que l’utilisateur utilise le même compte pour accepter l’invitation et se connecter au site.</span><span class="sxs-lookup"><span data-stu-id="33d94-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="33d94-107">Pour plus d’informations, reportez-vous à la rubrique [How</a> to Manage aliases for Your Microsoft Account pour gérer la connexion Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="33d94-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="33d94-108">Accédez à chaque site (s) dans lequel l’utilisateur reçoit l’erreur.</span><span class="sxs-lookup"><span data-stu-id="33d94-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="33d94-109">Ajoutez « /_layouts/15/People.aspx/MembershipGroupId = 0 » (dans les guillemets doubles) à la fin de l’URL du site.</span><span class="sxs-lookup"><span data-stu-id="33d94-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="33d94-110">Exemple : https://< « contoso » >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="33d94-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="33d94-111">Sélectionnez l’utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="33d94-111">Select the user from the list.</span></span>

- <span data-ttu-id="33d94-112">Cliquez sur **Supprimer les autorisations des utilisateurs** du ruban.</span><span class="sxs-lookup"><span data-stu-id="33d94-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="33d94-113">Rajoutez l’utilisateur et renvoyez-le à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="33d94-113">Add back the User and Resend the invite to the user.</span></span>

