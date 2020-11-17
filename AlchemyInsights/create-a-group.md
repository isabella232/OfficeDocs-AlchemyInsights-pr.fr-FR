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
# <a name="create-a-group"></a>Créer un groupe

Cette rubrique décrit la création de groupes.

**Autorisation de créer un groupe**

Assurez-vous que vous êtes autorisé à créer un groupe. Les administrateurs globaux peuvent désactiver la création de groupes dans le portail Azure ou dans le panneau d’accès. Vous aurez peut-être besoin d’un administrateur pour créer le groupe pour vous ou pour vous accorder les autorisations appropriées.

**Gérer les autorisations de création de groupe**

1. Les administrateurs généraux peuvent gérer les autorisations de création de groupe (pour des raisons liées à la sécurité) ou les groupes Office 365 créés dans le portail Azure ou le panneau d’accès, en choisissant les options « les utilisateurs peuvent créer des groupes de sécurité dans les portails Azure » ou « les utilisateurs peuvent créer des groupes Office 365 dans Azure Portals » dans **tous les groupes**  >  **général (paramètres)**.
2. Vous pouvez également limiter la création de groupe pour sélectionner un groupe d’utilisateurs si vous disposez d’une licence Azure Active Directory P1 Premium.

**Désactivation de la notification de bienvenue pour les nouveaux membres du groupe Office 365**

Les notifications de bienvenue envoyées aux utilisateurs ajoutés aux groupes Office 365 peuvent être désactivées en affectant la valeur false à **UnifiedGroupWelcomeMessageEnabled** dans PowerShell. Découvrez ce paramètre [ici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

