---
title: Dépannage des messages refusés d’accès aux sites OneDrive entreprise
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692799"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="292ae-102">Dépannage des messages refusés d’accès aux sites OneDrive entreprise</span><span class="sxs-lookup"><span data-stu-id="292ae-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="292ae-103">Ce problème se produit le plus souvent lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="292ae-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="292ae-104">Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente.</span><span class="sxs-lookup"><span data-stu-id="292ae-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="292ae-105">Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect.</span><span class="sxs-lookup"><span data-stu-id="292ae-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="292ae-106">Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory.</span><span class="sxs-lookup"><span data-stu-id="292ae-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="292ae-107">Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.</span><span class="sxs-lookup"><span data-stu-id="292ae-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="292ae-108">Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article [restaurer un utilisateur dans Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="292ae-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="292ae-109">Si vous ne pouvez pas restaurer l’utilisateur d’origine, vous devez supprimer l’ancien utilisateur du site OneDrive en suivant ces étapes, [supprimer un utilisateur de la liste d’informations utilisateur]().</span><span class="sxs-lookup"><span data-stu-id="292ae-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="292ae-110">Une fois cette opération terminée, vous pouvez vérifier que l’utilisateur dispose de droits d’administrateur sur le site OneDrive en suivant les étapes d’ajout de l' [administrateur pour le onedrive d’un utilisateur](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="292ae-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="292ae-111">Pour plus d’informations sur les niveaux d’autorisation, voir l’article relatif aux [niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="292ae-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
