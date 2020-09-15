---
title: Résoudre l’erreur de connexion Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687036"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="f4826-102">Résoudre l’erreur de connexion Teams AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="f4826-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="f4826-103">Lorsque vous vous connectez à Microsoft Teams, le message d’erreur suivant peut s’afficher : **Désolé... Nous rencontrons des difficultés pour vous connecter à AADSTS9000411 : la demande n’est pas correctement mise en forme. Le paramètre « login_hint » est dupliqué.**</span><span class="sxs-lookup"><span data-stu-id="f4826-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="f4826-104">Pour résoudre ce problème, assurez-vous que vos clients Microsoft Teams sont mis à jour.</span><span class="sxs-lookup"><span data-stu-id="f4826-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="f4826-105">Pour plus d’informations sur la mise à jour de votre client, voir [Mettre à jour Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f4826-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="f4826-106">Si vous ne pouvez pas mettre à jour votre client pour une raison quelconque, la déconnexion du client efface la plupart des données mises en cache.</span><span class="sxs-lookup"><span data-stu-id="f4826-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="f4826-107">Toutefois, si vous rencontrez encore des problèmes après la fermeture et l’ouverture de session, quittez Teams et effacez le cache de votre client en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="f4826-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="f4826-108">Fermez Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f4826-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="f4826-109">Accédez à :%appdata%\microsoft\teams et supprimez tous les fichiers.</span><span class="sxs-lookup"><span data-stu-id="f4826-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="f4826-110">Ouvrir Microsoft Teams de nouveau.</span><span class="sxs-lookup"><span data-stu-id="f4826-110">Reopen Microsoft Teams.</span></span>
