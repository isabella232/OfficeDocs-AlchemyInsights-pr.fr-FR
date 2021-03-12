---
title: Résoudre les problèmes de messages d’accès refusé
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707952"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="216aa-102">Résoudre les problèmes de messages d’accès refusé dans le Centre d’administration Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="216aa-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="216aa-103">Si vous recevez un message de refus d’accès lors de la tentative d’accès à un Centre d’administration Sharepoint/OneDrive, assurez-vous d’attribuer une licence [à l’utilisateur.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="216aa-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="216aa-104">Si l’utilisateur dispose d’une licence, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) vous devez également vous assurer qu’un rôle d’administrateur lui est attribué et qu’il peut accéder aux centres d’administration.</span><span class="sxs-lookup"><span data-stu-id="216aa-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="216aa-105">Ce problème peut également se produire lorsqu’un utilisateur est supprimé et re-créé avec le même nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="216aa-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="216aa-106">Le nouveau compte est créé à l’aide d’une autre valeur PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="216aa-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="216aa-107">Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, il dispose d’un PUID incorrect.</span><span class="sxs-lookup"><span data-stu-id="216aa-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="216aa-108">Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory.</span><span class="sxs-lookup"><span data-stu-id="216aa-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="216aa-109">Si les utilisateurs se sont déjà inscrits à SharePoint, puis sont déplacés vers une autre ouo et resyncés avec SharePoint, ils peuvent être face à ce problème.</span><span class="sxs-lookup"><span data-stu-id="216aa-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="216aa-110">Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes de l’article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="216aa-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="216aa-111">Remarque : si un centre d’administration OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui y avaient précédemment accès, il peut y avoir un problème de service temporaire.</span><span class="sxs-lookup"><span data-stu-id="216aa-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="216aa-112">[Vérifiez le tableau de bord d’état du service.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="216aa-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


