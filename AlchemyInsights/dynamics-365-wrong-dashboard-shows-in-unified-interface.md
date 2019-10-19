---
title: Dynamics 365-tableau de bord incorrect dans Dynamics 365 Unified interface
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528549"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Tableau de bord incorrect dans l’interface unifiée Dynamics 365

Il existe plusieurs raisons pour lesquelles vous pouvez voir un tableau de bord différent de celui que vous attendez :

## <a name="the-user-has-set-a-user-default-dashboard"></a>L’utilisateur a défini un tableau de bord par défaut de l’utilisateur 

En règle générale, vous pouvez identifier un tableau de bord par défaut de l’utilisateur est défini si le bouton **définir par défaut** n’est pas affiché dans la barre de commandes tableau de bord. Le tableau de bord par défaut de l’utilisateur remplacera tous les autres tableaux de bord par défaut, même si le tableau de bord par défaut de l’utilisateur ne se trouve pas dans l’application actuelle.

Utilisez la solution de contournement suivante pour annuler le tableau de bord par défaut.

1. Créez un tableau de bord personnel.

2. Définissez le nouveau tableau de bord comme utilisateur par défaut.

3. Supprimez ce tableau de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Le tableau de bord est défini dans le sitemap.

Vous avez peut-être défini un tableau de bord par défaut de l’organisation en sélectionnant un tableau de bord et en choisissant « définir par défaut » sous « personnaliser le système ». Toutefois, le tableau de bord défini dans le concepteur Sitemap est prioritaire sur ce tableau de bord, si l’utilisateur y a accès.

Pour que les utilisateurs voient le tableau de bord que vous avez défini en tant qu’organisation par défaut, vous pouvez :

* Définir ce tableau de bord dans le plan de sitemap

* Supprimer l’accès au tableau de bord défini sitemap pour ces utilisateurs
