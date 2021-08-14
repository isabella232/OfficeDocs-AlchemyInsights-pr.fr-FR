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
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945740"
---
# <a name="hide-public-folders"></a>Masquer les dossiers publics.

**Pour masquer l’arborescence de dossiers publics** :

Utilisez les étapes de [cet](https://aka.ms/ControlPF) article pour masquer l’arborescence de dossiers publics à des utilisateurs spécifiques ou à tous les utilisateurs.

**Pour masquer un dossier public spécifique** :

1. Ajouter des autorisations pour les utilisateurs qui ont besoin d’accéder au dossier public

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Supprimez la valeur **Par défaut** de l’utilisateur de la liste des **Autorisations** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
