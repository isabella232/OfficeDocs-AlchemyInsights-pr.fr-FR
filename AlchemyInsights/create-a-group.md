---
title: Créer un groupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816346"
---
# <a name="create-a-group"></a><span data-ttu-id="7a189-102">Créer un groupe</span><span class="sxs-lookup"><span data-stu-id="7a189-102">Create a group</span></span>

<span data-ttu-id="7a189-103">Cette rubrique décrit la création de groupes.</span><span class="sxs-lookup"><span data-stu-id="7a189-103">This topic describes group creation.</span></span>

<span data-ttu-id="7a189-104">**Autorisation de créer un groupe**</span><span class="sxs-lookup"><span data-stu-id="7a189-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="7a189-105">Assurez-vous que vous êtes autorisé à créer un groupe.</span><span class="sxs-lookup"><span data-stu-id="7a189-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="7a189-106">Les administrateurs généraux peuvent désactiver la création de groupes dans le Portail Azure ou le panneau d’accès.</span><span class="sxs-lookup"><span data-stu-id="7a189-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="7a189-107">Il se peut que vous ayez besoin d'un administrateur pour créer le nouveau groupe pour vous, ou pour vous donner les autorisations appropriées.</span><span class="sxs-lookup"><span data-stu-id="7a189-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="7a189-108">**Gérer les autorisations de création de groupes**</span><span class="sxs-lookup"><span data-stu-id="7a189-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="7a189-109">Les administrateurs généraux peuvent gérer les autorisations de création de groupes (pour des raisons de sécurité) ou les groupes Office 365 créés dans le portail Azure ou le Panneau d'accès, en choisissant les options « Les utilisateurs peuvent créer des groupes de sécurité dans les portails Azure » ou « Les utilisateurs peuvent créer des groupes Office 365 dans les portails Azure » dans Tous les groupes Général  >  **(Paramètres).**</span><span class="sxs-lookup"><span data-stu-id="7a189-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="7a189-110">Vous pouvez également restreindre la création de groupes pour sélectionner un groupe d'utilisateurs si vous avez une licence Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="7a189-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="7a189-111">**Désactivation de la notification d'accueil pour les nouveaux membres du groupe Office 365**</span><span class="sxs-lookup"><span data-stu-id="7a189-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="7a189-112">La notification de bienvenue envoyée aux utilisateurs ajoutés aux groupes Office 365 peut être désactivée en activant **UnifiedGroupWelcomeMessageEnabled** sur False dans Powershell.</span><span class="sxs-lookup"><span data-stu-id="7a189-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="7a189-113">En savoir plus sur ce paramètre [ici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="7a189-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

