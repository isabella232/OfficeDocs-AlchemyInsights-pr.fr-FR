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
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="d1eb5-102">Le graphique affiche un nombre différent d’enregistrements dans la grille</span><span class="sxs-lookup"><span data-stu-id="d1eb5-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="d1eb5-103">**Symptôme**</span><span class="sxs-lookup"><span data-stu-id="d1eb5-103">**Symptom**</span></span>

<span data-ttu-id="d1eb5-104">Pour graphique sur la page du tableau de bord, lorsque vous cliquez sur le graphique « ... » et cliquer sur « Afficher les enregistrements », vous accédez à la page grille pour afficher tous les enregistrements. Il peut arriver que le nombre d’enregistrements change.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="d1eb5-105">**Cause**</span><span class="sxs-lookup"><span data-stu-id="d1eb5-105">**Cause**</span></span>

<span data-ttu-id="d1eb5-106">Ceci est dû à la différence des affichages entre le graphique dans la page de tableau de bord d’origine et le graphique sur la page d’accueil de la grille.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="d1eb5-107">**Solution**</span><span class="sxs-lookup"><span data-stu-id="d1eb5-107">**Solution**</span></span>

1. <span data-ttu-id="d1eb5-108">Vérifiez l’affichage de la page d’origine et l’affichage dans la grille pour voir s’ils sont différents.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="d1eb5-109">Modifiez l’affichage dans la grille pour qu’il corresponde à l’affichage dans la page d’origine.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="d1eb5-110">Si l’affichage correct est introuvable, cela signifie généralement que l’affichage n’est pas activé dans le concepteur d’applications.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="d1eb5-111">Accédez au concepteur d’applications de l’application spécifique, sélectionnez l’entité et ses affichages, vérifiez l’affichage que vous voulez activer, enregistrer, publier et fermer.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="d1eb5-112">Actualisez la page.</span><span class="sxs-lookup"><span data-stu-id="d1eb5-112">Refresh the page.</span></span>