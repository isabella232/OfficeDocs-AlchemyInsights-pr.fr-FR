---
title: 0x8004de40'erreur lors du lancement de OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813650"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="7c36c-102">0x8004de40'erreur lors du lancement de OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c36c-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="7c36c-103">Si vous recevez un message **d'0x8004de40** lors de la connexion à OneDrive, redémarrez l'ordinateur lorsque vous êtes connecté à votre domaine scolaire ou scolaire.</span><span class="sxs-lookup"><span data-stu-id="7c36c-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="7c36c-104">Si vous recevez cette erreur après le redémarrage, essayez ceci lorsque vous êtes connecté à votre domaine scolaire ou scolaire :</span><span class="sxs-lookup"><span data-stu-id="7c36c-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="7c36c-105">Cliquez sur Démarrer, puis tapez **cmd** **ou** invite de commandes dans la zone de recherche, cliquez avec le bouton droit sur l'application d'invite de commandes, puis sélectionnez Exécuter en **tant qu'administrateur.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="7c36c-106">Si vous êtes invité à obtenir un mot de passe d'administrateur ou une confirmation, tapez le mot de passe ou cliquez sur **Autoriser.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="7c36c-107">Dans la fenêtre Invite de commandes, tapez **dsregcmd /leave**  et attendez que la commande se termine.</span><span class="sxs-lookup"><span data-stu-id="7c36c-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="7c36c-108">Tapez **ensuite dsregcmd /join** et attendez la fin de la commande.</span><span class="sxs-lookup"><span data-stu-id="7c36c-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="7c36c-109">Redémarrez votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="7c36c-109">Reboot your computer.</span></span>
