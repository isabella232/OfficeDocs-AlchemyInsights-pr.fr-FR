---
title: Le graphique affiche un nombre différent d’enregistrements dans la grille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431453"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>Le graphique affiche un nombre différent d’enregistrements dans la grille

**Symptôme**

Pour graphique sur la page du tableau de bord, lorsque vous cliquez sur le graphique « ... » et cliquer sur « Afficher les enregistrements », vous accédez à la page grille pour afficher tous les enregistrements. Il peut arriver que le nombre d’enregistrements change.

**Cause**

Ceci est dû à la différence des affichages entre le graphique dans la page de tableau de bord d’origine et le graphique sur la page d’accueil de la grille.  

**Solution**

1. Vérifiez l’affichage de la page d’origine et l’affichage dans la grille pour voir s’ils sont différents.
2. Modifiez l’affichage dans la grille pour qu’il corresponde à l’affichage dans la page d’origine.
3. Si l’affichage correct est introuvable, cela signifie généralement que l’affichage n’est pas activé dans le concepteur d’applications.
4. Accédez au concepteur d’applications de l’application spécifique, sélectionnez l’entité et ses affichages, vérifiez l’affichage que vous voulez activer, enregistrer, publier et fermer.
5. Actualisez la page.