---
title: Dynamics 365 - Tableau de bord erroné dans l’interface unifiée Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101480"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Tableau de bord erroné dans l’interface unifiée Dynamics 365

Il existe plusieurs raisons pour lesquelles vous pouvez voir un tableau de bord différent de celui prévu :

## <a name="the-user-has-set-a-user-default-dashboard"></a>L’utilisateur a définie un tableau de bord par défaut de l’utilisateur 

En règle générale, vous pouvez identifier  un tableau de bord par défaut de l’utilisateur si le bouton Définir comme valeur par défaut ne s’affiche pas dans la barre de commandes du tableau de bord. Le tableau de bord par défaut de l’utilisateur remplace tous les autres tableaux de bord par défaut, même si le tableau de bord par défaut de l’utilisateur ne se trouve pas dans l’application actuelle.

Utilisez la solution de contournement suivante pour déséseter leur tableau de bord par défaut.

1. Créez un tableau de bord personnel.

2. Définissez ce nouveau tableau de bord comme tableau de bord par défaut de l’utilisateur.

3. Supprimez ce tableau de bord.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Le tableau de bord est définie dans le plan de site

Vous avez peut-être créé un tableau de bord par défaut de l’organisation en sélectionnant un tableau de bord et en choisissant « Définir par défaut » sous « Personnaliser le système ». Toutefois, le tableau de bord défini dans le concepteur de plan de site sera prioritaire sur ce tableau de bord, si l’utilisateur y a accès.

Pour que les utilisateurs voient le tableau de bord que vous avez définie comme tableau de bord par défaut de l’organisation, vous pouvez :

* Définir ce tableau de bord dans le plan de site

* Supprimer l’accès au tableau de bord défini par sitemap pour ces utilisateurs
