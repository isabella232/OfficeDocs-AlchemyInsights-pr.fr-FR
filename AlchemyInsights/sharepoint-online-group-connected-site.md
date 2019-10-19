---
title: Ajouter un groupe à un site SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750518"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="8fa40-102">Problèmes lors de la création ou du regroupement de sites connectés dans SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8fa40-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="8fa40-103">Il existe deux problèmes courants lors de la création ou de la recréation d’un site connecté à un groupe.</span><span class="sxs-lookup"><span data-stu-id="8fa40-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="8fa40-104">Si vous avez supprimé un groupe et son site connecté et que vous souhaitez créer un autre site avec la même URL, vous devez supprimer définitivement le site précédent.</span><span class="sxs-lookup"><span data-stu-id="8fa40-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="8fa40-105">Télécharger [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="8fa40-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="8fa40-106">Pour plus d’informations sur la prise en main de PowerShell, voir [Getting Started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="8fa40-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="8fa40-107">Supprimez le site des sites supprimés à l’aide de l’applet de commande PowerShell [Remove-spodeletedsit](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="8fa40-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="8fa40-108">Si vous créez un site de groupe connecté et que vous recevez un avertissement, un autre groupe avec le même alias existe déjà, vérifiez les groupes existants à partir du [Centre d’administration Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="8fa40-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="8fa40-109">Pour résoudre le problème, supprimez le groupe existant s’il n’est plus nécessaire ou créez-en un autre.</span><span class="sxs-lookup"><span data-stu-id="8fa40-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="8fa40-110">Il existe différentes façons de créer et d’utiliser des groupes modernes avec SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8fa40-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="8fa40-111">Vous pouvez connecter des sites existants à un groupe Office 365.</span><span class="sxs-lookup"><span data-stu-id="8fa40-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="8fa40-112">Pour plus d’informations, consultez [la rubrique Connect an Office 365 Group using the SharePoint User ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="8fa40-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="8fa40-113">Pour créer un site connecté à un groupe Office 365, vous devez créer un site d’équipe.</span><span class="sxs-lookup"><span data-stu-id="8fa40-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="8fa40-114">Pour plus d’informations, consultez [la rubrique créer un site d’équipe dans SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="8fa40-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

