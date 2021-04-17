---
title: Résoudre les problèmes liés à OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826197"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6b1cc-102">Résoudre les problèmes liés à OneDrive</span><span class="sxs-lookup"><span data-stu-id="6b1cc-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6b1cc-103">Si OneDrive se bloque plusieurs fois, procédez comme suit pour résoudre les problèmes :</span><span class="sxs-lookup"><span data-stu-id="6b1cc-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6b1cc-104">**Vérifiez que les clés du Registre ne sont pas fixées :**</span><span class="sxs-lookup"><span data-stu-id="6b1cc-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6b1cc-105">À l’aide de l’Éditeur du Registre, accédez à HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6b1cc-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6b1cc-106">Si DisableFileSyncNGSC est présent et est paramétré définit sur 1, ouvrez la clé et modifiez la valeur sur 0.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6b1cc-107">Lancer manuellement OneDrive en accédant au menu Démarrer</span><span class="sxs-lookup"><span data-stu-id="6b1cc-107">Manually launch OneDrive by going to Start</span></span> ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6b1cc-109">, tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6b1cc-110">**Réinitialiser OneDrive :**</span><span class="sxs-lookup"><span data-stu-id="6b1cc-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6b1cc-111">Remarques :</span><span class="sxs-lookup"><span data-stu-id="6b1cc-111">Notes:</span></span>

- <span data-ttu-id="6b1cc-112">La réinitialisation de OneDrive déconnecte toutes vos connexions de synchronisation existantes (y compris de votre OneDrive personnel, s’il est configuré).</span><span class="sxs-lookup"><span data-stu-id="6b1cc-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6b1cc-113">La réinitialisation de OneDrive sur votre ordinateur n’entraîne pas de perte de fichiers ou de données.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6b1cc-114">**Pour réinitialiser OneDrive :**</span><span class="sxs-lookup"><span data-stu-id="6b1cc-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6b1cc-115">Ouvrez une boîte de dialogue Exécuter en appuyant sur la touche Windows et sur R.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6b1cc-116">Tapez %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, puis appuyez sur OK.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6b1cc-117">Une fenêtre Commande peut s’afficher brièvement.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6b1cc-118">Lancer manuellement OneDrive en accédant au menu Démarrer</span><span class="sxs-lookup"><span data-stu-id="6b1cc-118">Manually launch OneDrive by going to Start</span></span> ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6b1cc-120">, tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6b1cc-121">Remarques :</span><span class="sxs-lookup"><span data-stu-id="6b1cc-121">Notes:</span></span>

- <span data-ttu-id="6b1cc-122">Si vous aviez choisi de ne synchroniser que quelques dossiers avant la réinitialisation, vous devrez recommencer une fois la synchronisation terminée.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6b1cc-123">Pour plus d’informations, lisez  [Choisir quels dossiers OneDrive synchroniser avec votre ordinateur](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .</span><span class="sxs-lookup"><span data-stu-id="6b1cc-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6b1cc-124">Vous devrez effectuer cette opération pour votre espace OneDrive Personnel et OneDrive Entreprise.</span><span class="sxs-lookup"><span data-stu-id="6b1cc-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>