---
title: Résoudre Bluetooth problèmes liés à Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812930"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="7b9c2-102">Résoudre Bluetooth problèmes liés à Windows 10</span><span class="sxs-lookup"><span data-stu-id="7b9c2-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="7b9c2-103">Si l'icône Bluetooth est manquante ou si Bluetooth ne peut pas être désactivé, vous pouvez exécuter l'Bluetooth dépannage.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="7b9c2-104">[Ouvrez les paramètres de](ms-settings:troubleshoot)résolution des problèmes, cliquez **Bluetooth** sous **Rechercher** et résoudre les autres problèmes, cliquez sur **Exécuter l'dépannage.**</span><span class="sxs-lookup"><span data-stu-id="7b9c2-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="7b9c2-105">Si vous ne voyez pas l'icône Bluetooth, mais Bluetooth s'affiche dans le Gestionnaire de périphériques :</span><span class="sxs-lookup"><span data-stu-id="7b9c2-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="7b9c2-106">Dans le Gestionnaire de périphériques, **cliquez sur Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="7b9c2-107">Appuyez de nouveau (ou cliquez avec le bouton droit) sur le Bluetooth adaptateur et cliquez **sur Désinstaller l'appareil.**</span><span class="sxs-lookup"><span data-stu-id="7b9c2-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="7b9c2-108">Fermez votre appareil Windows, patientez quelques secondes, puis r allumez-le.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="7b9c2-109">Windows essaiera de réinstaller le pilote.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="7b9c2-110">Si vous avez récemment installé les mises à jour Windows 10 ou mis à niveau vers Windows 10, vous pouvez vérifier les mises à jour des pilotes :</span><span class="sxs-lookup"><span data-stu-id="7b9c2-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="7b9c2-111">Dans le Gestionnaire de périphériques, cliquez **Bluetooth,** puis cliquez sur le nom Bluetooth adaptateur (qui peut inclure le mot « radio »).</span><span class="sxs-lookup"><span data-stu-id="7b9c2-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="7b9c2-112">Appuyez avec le bouton droit de la souris (ou cliquez avec le bouton droit) sur la carte Bluetooth, puis cliquez sur Mettre à jour automatiquement le pilote de recherche pour les  >  **logiciels de pilotes mis à jour.**</span><span class="sxs-lookup"><span data-stu-id="7b9c2-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="7b9c2-113">Suivez les étapes, puis cliquez sur **Fermer.**</span><span class="sxs-lookup"><span data-stu-id="7b9c2-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="7b9c2-114">Si Windows ne trouve pas de nouveau pilote Bluetooth, visitez le site web du fabricant du PC et téléchargez le dernier pilote Bluetooth à partir de là.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="7b9c2-115">Après l'avoir téléchargé, cliquez sur Mettre à jour le pilote Parcourir mon ordinateur pour rechercher le logiciel de pilote Recherchez l'emplacement où les fichiers de pilotes sont stockés > OK Suivant, puis suivez les étapes  >    >     >  d'installation.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="7b9c2-116">Après avoir installé le pilote mis à jour, redémarrez l'ordinateur, puis vérifiez si cela résout le problème de connexion.</span><span class="sxs-lookup"><span data-stu-id="7b9c2-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="7b9c2-117">Pour plus d'informations sur la résolution des problèmes de Bluetooth, consultez l'article complet, Résoudre Bluetooth problèmes dans [Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="7b9c2-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
