---
title: erreur 0x8004de40 lors du lancement de OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815991"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="1259a-102">erreur 0x8004de40 lors du lancement de OneDrive</span><span class="sxs-lookup"><span data-stu-id="1259a-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="1259a-103">Si vous recevez un message d’erreur **0x8004de40** lors de la connexion à OneDrive, redémarrez l’ordinateur tout en étant connecté à votre domaine professionnel ou scolaire.</span><span class="sxs-lookup"><span data-stu-id="1259a-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="1259a-104">Si vous recevez cette erreur après avoir redémarré, essayez ceci en vous connectant à votre domaine professionnel ou scolaire :</span><span class="sxs-lookup"><span data-stu-id="1259a-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="1259a-105">Cliquez sur Démarrer, puis tapez **cmd** ou **invite de commandes**  dans la zone de recherche, cliquez avec le bouton droit sur l’application invite de commandes, puis sélectionnez  **exécuter en tant qu’administrateur** .</span><span class="sxs-lookup"><span data-stu-id="1259a-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="1259a-106">Si vous êtes invité à entrer un mot de passe d’administrateur ou une confirmation, tapez le mot de passe, ou cliquez sur **autoriser** .</span><span class="sxs-lookup"><span data-stu-id="1259a-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="1259a-107">Dans la fenêtre d’invite de commandes, tapez **dsregcmd/Leave**  et attendez la fin de la commande.</span><span class="sxs-lookup"><span data-stu-id="1259a-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="1259a-108">Tapez ensuite **dsregcmd/Join** et attendez la fin de la commande.</span><span class="sxs-lookup"><span data-stu-id="1259a-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="1259a-109">Redémarrez votre ordinateur.</span><span class="sxs-lookup"><span data-stu-id="1259a-109">Reboot your computer.</span></span>
