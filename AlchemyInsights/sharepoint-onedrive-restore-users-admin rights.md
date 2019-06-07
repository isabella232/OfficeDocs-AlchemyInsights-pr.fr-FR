---
title: Donner aux utilisateurs l’accès à SharePoint et OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759254"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="ea26b-102">Donner aux utilisateurs l’accès à SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="ea26b-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="ea26b-103">Ce problème se produit le plus souvent lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="ea26b-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ea26b-104">Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente.</span><span class="sxs-lookup"><span data-stu-id="ea26b-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ea26b-105">Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect.</span><span class="sxs-lookup"><span data-stu-id="ea26b-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ea26b-106">Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea26b-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ea26b-107">Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.</span><span class="sxs-lookup"><span data-stu-id="ea26b-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ea26b-108">Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article[restaurer un utilisateur dans Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ea26b-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="ea26b-109">Une fois cette opération terminée, vous pouvez vérifier que l’utilisateur dispose de droits d’administrateur sur le site OneDrive en suivant les étapes d’ajout de l' [administrateur pour le onedrive d’un utilisateur](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) .</span><span class="sxs-lookup"><span data-stu-id="ea26b-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="ea26b-110">Pour plus d’informations sur les niveaux d’autorisation, voir l’article relatif aux [niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="ea26b-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
