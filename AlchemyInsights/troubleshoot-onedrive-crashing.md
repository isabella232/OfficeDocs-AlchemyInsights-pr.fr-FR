---
title: Résoudre les problèmes liés à OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44735389"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="4f3fa-102">Résoudre les problèmes liés à OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f3fa-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="4f3fa-103">Si OneDrive se bloque plusieurs fois, procédez comme suit pour résoudre les problèmes :</span><span class="sxs-lookup"><span data-stu-id="4f3fa-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="4f3fa-104">**Vérifiez que les clés du Registre ne sont pas fixées :**</span><span class="sxs-lookup"><span data-stu-id="4f3fa-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="4f3fa-105">À l’aide de l’Éditeur du Registre, accédez à HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f3fa-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="4f3fa-106">Si DisableFileSyncNGSC est présent et est paramétré définit sur 1, ouvrez la clé et modifiez la valeur sur 0.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="4f3fa-107">Lancer manuellement OneDrive en accédant au menu Démarrer</span><span class="sxs-lookup"><span data-stu-id="4f3fa-107">Manually launch OneDrive by going to Start</span></span> ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4f3fa-109">, tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4f3fa-110">**Réinitialiser OneDrive :**</span><span class="sxs-lookup"><span data-stu-id="4f3fa-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="4f3fa-111">Remarques :</span><span class="sxs-lookup"><span data-stu-id="4f3fa-111">Notes:</span></span>

- <span data-ttu-id="4f3fa-112">La réinitialisation de OneDrive déconnecte toutes vos connexions de synchronisation existantes (y compris de votre OneDrive personnel, s’il est configuré).</span><span class="sxs-lookup"><span data-stu-id="4f3fa-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="4f3fa-113">La réinitialisation de OneDrive sur votre ordinateur n’entraîne pas de perte de fichiers ou de données.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="4f3fa-114">**Pour réinitialiser OneDrive :**</span><span class="sxs-lookup"><span data-stu-id="4f3fa-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="4f3fa-115">Ouvrez une boîte de dialogue Exécuter en appuyant sur la touche Windows et sur R.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="4f3fa-116">Tapez %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, puis appuyez sur OK.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="4f3fa-117">Une fenêtre Commande peut s’afficher brièvement.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="4f3fa-118">Lancer manuellement OneDrive en accédant au menu Démarrer</span><span class="sxs-lookup"><span data-stu-id="4f3fa-118">Manually launch OneDrive by going to Start</span></span> ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="4f3fa-120">, tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="4f3fa-121">Remarques :</span><span class="sxs-lookup"><span data-stu-id="4f3fa-121">Notes:</span></span>

- <span data-ttu-id="4f3fa-122">Si vous aviez choisi de ne synchroniser que quelques dossiers avant la réinitialisation, vous devrez recommencer une fois la synchronisation terminée.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="4f3fa-123">Pour plus d’informations, lisez  [Choisir quels dossiers OneDrive synchroniser avec votre ordinateur](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .</span><span class="sxs-lookup"><span data-stu-id="4f3fa-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="4f3fa-124">Vous devrez effectuer cette opération pour votre espace OneDrive Personnel et OneDrive Entreprise.</span><span class="sxs-lookup"><span data-stu-id="4f3fa-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>