---
title: Masquer les dossiers publics.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50294641"
---
# <a name="hide-public-folders"></a><span data-ttu-id="86e7d-102">Masquer les dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="86e7d-102">Hide public folders</span></span>

<span data-ttu-id="86e7d-103">**Pour masquer l’arborescence de dossiers publics** :</span><span class="sxs-lookup"><span data-stu-id="86e7d-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="86e7d-104">Utilisez les étapes de [cet](https://aka.ms/ControlPF) article pour masquer l’arborescence de dossiers publics à des utilisateurs spécifiques ou à tous les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="86e7d-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="86e7d-105">**Pour masquer un dossier public spécifique** :</span><span class="sxs-lookup"><span data-stu-id="86e7d-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="86e7d-106">Ajouter des autorisations pour les utilisateurs qui ont besoin d’accéder au dossier public</span><span class="sxs-lookup"><span data-stu-id="86e7d-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="86e7d-107">Supprimez la valeur **Par défaut** de l’utilisateur de la liste des **Autorisations** :</span><span class="sxs-lookup"><span data-stu-id="86e7d-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
