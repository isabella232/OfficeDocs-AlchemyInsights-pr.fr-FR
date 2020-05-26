---
title: Exécuter les Diagnostics de mémoire Windows dans Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289784"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="c7c98-102">Exécuter les Diagnostics de mémoire Windows dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="c7c98-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="c7c98-103">Si Windows et les applications de votre PC se bloquent, se figent ou agissent de manière instable, il se peut qu’il y ait un problème avec la mémoire vive (RAM) du PC.</span><span class="sxs-lookup"><span data-stu-id="c7c98-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="c7c98-104">Vous pouvez exécuter l’outil Diagnostic de mémoire Windows pour rechercher les problèmes liés à la mémoire vive du PC.</span><span class="sxs-lookup"><span data-stu-id="c7c98-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="c7c98-105">Dans la zone de recherche de la barre des tâches, tapez **Diagnostic de mémoire**, puis sélectionnez **Diagnostic de mémoire Windows**.</span><span class="sxs-lookup"><span data-stu-id="c7c98-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="c7c98-106">Pour exécuter le diagnostic, le PC doit redémarrer.</span><span class="sxs-lookup"><span data-stu-id="c7c98-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="c7c98-107">Vous avez la possibilité de redémarrer immédiatement (veuillez tout d’abord enregistrer votre travail, fermer les documents et les messages électroniques ouverts), ou de planifier l’exécution automatique du diagnostic lors du prochain démarrage de l’ordinateur :</span><span class="sxs-lookup"><span data-stu-id="c7c98-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Diagnostic de mémoire Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="c7c98-109">Lorsque le PC redémarre, l’**Outil Diagnostics de mémoire Windows** s’exécute automatiquement.</span><span class="sxs-lookup"><span data-stu-id="c7c98-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="c7c98-110">L’État et la progression s’affichent pendant l’exécution des diagnostics, et vous pouvez annuler les diagnostics en appuyant sur la touche **Échap** de votre clavier.</span><span class="sxs-lookup"><span data-stu-id="c7c98-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="c7c98-111">Une fois les diagnostics terminés, Windows démarre normalement.</span><span class="sxs-lookup"><span data-stu-id="c7c98-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="c7c98-112">Immédiatement après le redémarrage, lorsque le Bureau s’affiche, une notification apparaît (à côté de l’icône du **Centre de notifications** dans la barre des tâches) pour indiquer si des erreurs de mémoire ont été détectées.</span><span class="sxs-lookup"><span data-stu-id="c7c98-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="c7c98-113">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="c7c98-113">For example:</span></span>

<span data-ttu-id="c7c98-114">Voici l’icône du Centre de notifications :</span><span class="sxs-lookup"><span data-stu-id="c7c98-114">Here's the Action Center icon:</span></span> ![Icône du Centre de notifications](media/action-center-icon.png) 

<span data-ttu-id="c7c98-116">Et un exemple de notification :</span><span class="sxs-lookup"><span data-stu-id="c7c98-116">And a sample notification:</span></span> ![Aucune erreur de mémoire](media/no-memory-errors.png)

<span data-ttu-id="c7c98-118">Si vous n’avez pas vu la notification, vous pouvez sélectionner l’icône du **Centre de notifications** dans la barre des tâches pour afficher le **Centre de notifications** et une liste déroulante des notifications.</span><span class="sxs-lookup"><span data-stu-id="c7c98-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="c7c98-119">Pour consulter des informations détaillées, tapez **Évènements** dans la zone de recherche de la barre des tâches, puis sélectionnez **Observateur d’évènements**.</span><span class="sxs-lookup"><span data-stu-id="c7c98-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="c7c98-120">Dans le volet gauche de l’**Observateur d’évènements**, accédez à **Journaux Windows > Système**.</span><span class="sxs-lookup"><span data-stu-id="c7c98-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="c7c98-121">Dans le volet droit, parcourez la liste en examinant la colonne **Source**, jusqu’à ce que vous voyez les événements ayant pour valeur Source **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="c7c98-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="c7c98-122">Sélectionnez chacun de ces événements et consultez les informations du résultat dans la zone située sous l’onglet **Général** en dessous de la liste.</span><span class="sxs-lookup"><span data-stu-id="c7c98-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
