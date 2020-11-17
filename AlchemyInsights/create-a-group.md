---
title: Créer un groupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086289"
---
# <a name="create-a-group"></a><span data-ttu-id="85c06-102">Créer un groupe</span><span class="sxs-lookup"><span data-stu-id="85c06-102">Create a group</span></span>

<span data-ttu-id="85c06-103">Cette rubrique décrit la création de groupes.</span><span class="sxs-lookup"><span data-stu-id="85c06-103">This topic describes group creation.</span></span>

<span data-ttu-id="85c06-104">**Autorisation de créer un groupe**</span><span class="sxs-lookup"><span data-stu-id="85c06-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="85c06-105">Assurez-vous que vous êtes autorisé à créer un groupe.</span><span class="sxs-lookup"><span data-stu-id="85c06-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="85c06-106">Les administrateurs globaux peuvent désactiver la création de groupes dans le portail Azure ou dans le panneau d’accès.</span><span class="sxs-lookup"><span data-stu-id="85c06-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="85c06-107">Vous aurez peut-être besoin d’un administrateur pour créer le groupe pour vous ou pour vous accorder les autorisations appropriées.</span><span class="sxs-lookup"><span data-stu-id="85c06-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="85c06-108">**Gérer les autorisations de création de groupe**</span><span class="sxs-lookup"><span data-stu-id="85c06-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="85c06-109">Les administrateurs généraux peuvent gérer les autorisations de création de groupe (pour des raisons liées à la sécurité) ou les groupes Office 365 créés dans le portail Azure ou le panneau d’accès, en choisissant les options « les utilisateurs peuvent créer des groupes de sécurité dans les portails Azure » ou « les utilisateurs peuvent créer des groupes Office 365 dans Azure Portals » dans **tous les groupes**  >  **général (paramètres)**.</span><span class="sxs-lookup"><span data-stu-id="85c06-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="85c06-110">Vous pouvez également limiter la création de groupe pour sélectionner un groupe d’utilisateurs si vous disposez d’une licence Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="85c06-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="85c06-111">**Désactivation de la notification de bienvenue pour les nouveaux membres du groupe Office 365**</span><span class="sxs-lookup"><span data-stu-id="85c06-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="85c06-112">Les notifications de bienvenue envoyées aux utilisateurs ajoutés aux groupes Office 365 peuvent être désactivées en affectant la valeur false à **UnifiedGroupWelcomeMessageEnabled** dans PowerShell.</span><span class="sxs-lookup"><span data-stu-id="85c06-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="85c06-113">Découvrez ce paramètre [ici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="85c06-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

