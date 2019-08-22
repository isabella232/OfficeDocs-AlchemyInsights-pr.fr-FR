---
title: Résoudre les problèmes de refus d’accès aux messages
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503526"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="484c7-102">Résoudre les problèmes de refus d’accès aux messages dans le centre d’administration SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="484c7-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="484c7-103">Si vous recevez un message de refus d’accès lorsque vous tentez d’accéder à un centre d’administration SharePoint/OneDrive, veillez [à attribuer une licence à l’utilisateur](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="484c7-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="484c7-104">Si l’utilisateur dispose d’une licence, vous devez également vous assurer qu’il dispose [d’un rôle d’administrateur](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) pouvant accéder aux centres d’administration.</span><span class="sxs-lookup"><span data-stu-id="484c7-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="484c7-105">Ce problème peut également se produire lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="484c7-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="484c7-106">Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente.</span><span class="sxs-lookup"><span data-stu-id="484c7-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="484c7-107">Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect.</span><span class="sxs-lookup"><span data-stu-id="484c7-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="484c7-108">Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory.</span><span class="sxs-lookup"><span data-stu-id="484c7-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="484c7-109">Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.</span><span class="sxs-lookup"><span data-stu-id="484c7-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="484c7-110">Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article [restaurer un utilisateur dans Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="484c7-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="484c7-111">Remarque: si un centre d’administration OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs ayant précédemment accès, il peut y avoir un problème de service temporaire.</span><span class="sxs-lookup"><span data-stu-id="484c7-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="484c7-112">[Vérifiez le tableau de bord d’État du service](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="484c7-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


