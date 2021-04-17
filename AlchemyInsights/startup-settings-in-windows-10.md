---
title: Paramètres de démarrage dans Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828150"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="bec77-102">Paramètres de démarrage dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="bec77-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="bec77-103">**Modifier les applications qui s'exécutent automatiquement au démarrage**</span><span class="sxs-lookup"><span data-stu-id="bec77-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="bec77-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="bec77-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="bec77-105">Assurez-vous que toutes les applications que vous souhaitez exécuter au démarrage sont **allumées.**</span><span class="sxs-lookup"><span data-stu-id="bec77-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="bec77-106">**Ajouter une application à exécuter automatiquement au démarrage**</span><span class="sxs-lookup"><span data-stu-id="bec77-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="bec77-107">Cliquez ou appuyez **sur Démarrer** et recherchez l'application que vous souhaitez exécuter au démarrage.</span><span class="sxs-lookup"><span data-stu-id="bec77-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="bec77-108">Cliquez avec le bouton droit sur l'application, cliquez **sur Plus,** puis cliquez **sur Ouvrir l'emplacement du fichier.**</span><span class="sxs-lookup"><span data-stu-id="bec77-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="bec77-109">Cela ouvre l'emplacement où le raccourci vers l'application est enregistré.</span><span class="sxs-lookup"><span data-stu-id="bec77-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="bec77-110">S'il n'existe aucune option pour ouvrir l'emplacement du fichier, cela signifie que l'application ne peut pas s'exécuter au démarrage.</span><span class="sxs-lookup"><span data-stu-id="bec77-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="bec77-111">Une fois l'emplacement du fichier ouvert, appuyez sur la touche **de logo Windows + R**, **tapez shell:startup,** puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="bec77-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="bec77-112">Le dossier De démarrage s'ouvre.</span><span class="sxs-lookup"><span data-stu-id="bec77-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="bec77-113">Copiez et collez le raccourci vers l'application à partir de l'emplacement du fichier dans le dossier De démarrage.</span><span class="sxs-lookup"><span data-stu-id="bec77-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="bec77-114">**Options de démarrage avancées (y compris le mode sans échec, les paramètres UEFI et le démarrage à partir d'un autre appareil)**</span><span class="sxs-lookup"><span data-stu-id="bec77-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="bec77-115">Enregistrez votre travail et fermez les documents ouverts, car ces étapes redémarreront votre PC.</span><span class="sxs-lookup"><span data-stu-id="bec77-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="bec77-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="bec77-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="bec77-117">Sous **Démarrage avancé,** cliquez sur **Redémarrer maintenant.**</span><span class="sxs-lookup"><span data-stu-id="bec77-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="bec77-118">Une fois que votre PC a redémarré sur l'écran Choisir une option :</span><span class="sxs-lookup"><span data-stu-id="bec77-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="bec77-119">Pour démarrer à partir d'un appareil tel qu'un lecteur USB, cliquez **sur Utiliser un appareil.**</span><span class="sxs-lookup"><span data-stu-id="bec77-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="bec77-120">Pour entrer les paramètres UEFI (parfois appelés configuration du BIOS), cliquez sur Résoudre les problèmes > options avancées > paramètres du **microprogramme UEFI.**</span><span class="sxs-lookup"><span data-stu-id="bec77-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="bec77-121">Pour entrer en mode sans échec ou modifier les paramètres de démarrage avancés, cliquez sur Dépanner > Options avancées **> Paramètres** de démarrage, puis cliquez sur **Redémarrer.**</span><span class="sxs-lookup"><span data-stu-id="bec77-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="bec77-122">Vous pouvez être invité à entrer votre clé de récupération [BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="bec77-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="bec77-123">Après le redémarrage de votre PC, cliquez sur le paramètre de démarrage que vous souhaitez utiliser.</span><span class="sxs-lookup"><span data-stu-id="bec77-123">After your PC restarts again, click the startup setting you want to use.</span></span>