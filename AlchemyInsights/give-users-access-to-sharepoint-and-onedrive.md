---
title: Donner aux utilisateurs l’accès à SharePoint et OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677205"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="c8a49-102">Donner aux utilisateurs l’accès à SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="c8a49-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="c8a49-103">Si un site OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui disposaient précédemment d’un accès, il peut y avoir un problème de service temporaire.</span><span class="sxs-lookup"><span data-stu-id="c8a49-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="c8a49-104">Vérifier le tableau de bord d’État du service</span><span class="sxs-lookup"><span data-stu-id="c8a49-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="c8a49-105">Si vous souhaitez que les utilisateurs de votre organisation puissent se connecter et utiliser SharePoint et OneDrive, vous devez ajouter des comptes pour eux et vous assurer qu’ils disposent d’une licence leur permettant d’accéder à SharePoint et OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c8a49-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="c8a49-106">Le moyen le plus simple d’ajouter des utilisateurs se trouve dans le centre d’administration 365 de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c8a49-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="c8a49-107">Accédez à la [page utilisateurs actifs dans le centre d’administration Microsoft 365](https://portal.office.com/adminportal/home#/users), puis cliquez sur **Ajouter un utilisateur**.</span><span class="sxs-lookup"><span data-stu-id="c8a49-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="c8a49-108">Renseignez les informations de l’utilisateur et assurez-vous que sous **licences de produit**, une licence est attribuée et **SharePoint Online** est sélectionné.</span><span class="sxs-lookup"><span data-stu-id="c8a49-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="c8a49-109">Notez que si vous autorisez le partage externe dans votre organisation, les utilisateurs peuvent partager du contenu SharePoint et OneDrive avec des personnes extérieures à l’organisation.</span><span class="sxs-lookup"><span data-stu-id="c8a49-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="c8a49-110">Vous n’avez pas besoin d’accorder ces licences aux utilisateurs externes.</span><span class="sxs-lookup"><span data-stu-id="c8a49-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="c8a49-111">Vous n’avez pas non plus besoin d’ajouter des comptes pour ceux-ci, sauf si le partage est défini sur « uniquement les utilisateurs externes existants ».</span><span class="sxs-lookup"><span data-stu-id="c8a49-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="c8a49-112">Dans ce cas, si les personnes ne figurent pas dans l’annuaire de votre organisation, vous devez les ajouter en tant qu’utilisateurs invités dans le centre d’administration Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8a49-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

