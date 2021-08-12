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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929303"
---
# <a name="create-a-group"></a>Créer un groupe

Cette rubrique décrit la création de groupes.

**Autorisation de créer un groupe**

Assurez-vous que vous êtes autorisé à créer un groupe. Les administrateurs généraux peuvent désactiver la création de groupes dans le Portail Azure ou le panneau d’accès. Il se peut que vous ayez besoin d'un administrateur pour créer le nouveau groupe pour vous, ou pour vous donner les autorisations appropriées.

**Gérer les autorisations de création de groupes**

1. Les administrateurs généraux peuvent gérer les autorisations de création de groupes (pour des raisons de sécurité) ou les groupes Office 365 créés dans le portail Azure ou le Panneau d’accès, en choisissant les options « Les utilisateurs peuvent créer des groupes de sécurité dans les portails Azure » ou « Les utilisateurs peuvent créer des groupes Office 365 dans les portails Azure » dans Tous les groupes  >  **généraux (Paramètres).**
2. Vous pouvez également restreindre la création de groupes pour sélectionner un groupe d’utilisateurs si vous avez une licence Azure Active Directory P1 Premium.

**Désactivation de la notification d’accueil pour les nouveaux Office 365 groupe**

La notification de bienvenue envoyée aux utilisateurs ajoutés aux groupes Office 365 peut être désactivée en activant **UnifiedGroupWelcomeMessageEnabled** sur False dans Powershell. En savoir plus sur ce paramètre [ici](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

