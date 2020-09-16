---
title: Paramètres de démarrage dans Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751133"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="9593a-102">Paramètres de démarrage dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="9593a-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="9593a-103">**Modifier les applications qui s’exécutent automatiquement au démarrage**</span><span class="sxs-lookup"><span data-stu-id="9593a-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="9593a-104">Accédez à [paramètres > Apps > démarrage](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="9593a-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="9593a-105">Assurez-vous que toutes les applications que vous souhaitez exécuter au démarrage **sont activées.**</span><span class="sxs-lookup"><span data-stu-id="9593a-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="9593a-106">**Ajouter une application pour qu’elle s’exécute automatiquement au démarrage**</span><span class="sxs-lookup"><span data-stu-id="9593a-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="9593a-107">Cliquez ou appuyez sur **Démarrer** et recherchez l’application que vous souhaitez exécuter au démarrage.</span><span class="sxs-lookup"><span data-stu-id="9593a-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="9593a-108">Cliquez avec le bouton droit sur l’application, cliquez sur **plus**, puis sur **ouvrir l’emplacement du fichier**.</span><span class="sxs-lookup"><span data-stu-id="9593a-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="9593a-109">Cette action ouvre l’emplacement où le raccourci vers l’application est enregistré.</span><span class="sxs-lookup"><span data-stu-id="9593a-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="9593a-110">S’il n’existe pas d’option pour l’emplacement des fichiers ouverts, cela signifie que l’application ne peut pas être exécutée au démarrage.</span><span class="sxs-lookup"><span data-stu-id="9593a-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="9593a-111">Une fois l’emplacement du fichier ouvert, appuyez sur la **touche du logo Windows + R**, tapez **Shell : Startup**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="9593a-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="9593a-112">Le dossier démarrage s’ouvre.</span><span class="sxs-lookup"><span data-stu-id="9593a-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="9593a-113">Copiez et collez le raccourci vers l’application à partir de l’emplacement du fichier vers le dossier de démarrage.</span><span class="sxs-lookup"><span data-stu-id="9593a-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="9593a-114">**Options de démarrage avancées (y compris le mode sans échec, les paramètres UEFI et le démarrage à partir d’un autre périphérique)**</span><span class="sxs-lookup"><span data-stu-id="9593a-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="9593a-115">Enregistrez votre travail et fermez tous les documents ouverts, étant donné que ces étapes redémarreront votre PC.</span><span class="sxs-lookup"><span data-stu-id="9593a-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="9593a-116">Accédez à [paramètres > mise à jour & la récupération de la sécurité >](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="9593a-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="9593a-117">Sous **démarrage avancé**, cliquez sur **redémarrer maintenant**.</span><span class="sxs-lookup"><span data-stu-id="9593a-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="9593a-118">Après que votre PC a redémarré sur l’écran choisir une option, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="9593a-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="9593a-119">Pour démarrer à partir d’un appareil comme un lecteur USB, cliquez sur **utiliser un appareil**.</span><span class="sxs-lookup"><span data-stu-id="9593a-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="9593a-120">Pour entrer les paramètres UEFI (parfois appelés configuration du BIOS), cliquez sur **Troubleshoot > Advanced options > firmware UEFI Settings**.</span><span class="sxs-lookup"><span data-stu-id="9593a-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="9593a-121">Pour entrer en mode sans échec ou modifier les paramètres de démarrage avancés, cliquez sur **Troubleshoot > Advanced options > paramètres de démarrage**, puis sur **redémarrer**.</span><span class="sxs-lookup"><span data-stu-id="9593a-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="9593a-122">Vous serez peut-être invité à entrer votre [clé de récupération BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="9593a-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="9593a-123">Une fois que votre PC a redémarré, cliquez sur le paramètre de démarrage que vous souhaitez utiliser.</span><span class="sxs-lookup"><span data-stu-id="9593a-123">After your PC restarts again, click the startup setting you want to use.</span></span>