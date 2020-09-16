---
title: Corriger les problèmes Bluetooth dans Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730157"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="4cc41-102">Corriger les problèmes Bluetooth dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="4cc41-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="4cc41-103">Si l’icône Bluetooth est manquante ou si Bluetooth ne peut pas être activé ou désactivé, vous pouvez exécuter l’utilitaire de résolution des problèmes Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4cc41-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="4cc41-104">[Ouvrez les paramètres de résolution des problèmes](ms-settings:troubleshoot), cliquez sur **Bluetooth** sous **Rechercher et résoudre d’autres problèmes**, cliquez sur **exécuter l’utilitaire de résolution**des problèmes.</span><span class="sxs-lookup"><span data-stu-id="4cc41-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="4cc41-105">Si vous ne voyez pas l’icône Bluetooth, c’est que Bluetooth apparaît dans le gestionnaire de périphériques :</span><span class="sxs-lookup"><span data-stu-id="4cc41-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="4cc41-106">Dans le gestionnaire de périphériques, cliquez sur **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="4cc41-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="4cc41-107">Appuyez longuement (ou cliquez avec le bouton droit) sur le nom de la carte Bluetooth, puis cliquez sur **désinstaller l’appareil**.</span><span class="sxs-lookup"><span data-stu-id="4cc41-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="4cc41-108">Éteignez votre appareil Windows, patientez quelques secondes, puis rallumez-le.</span><span class="sxs-lookup"><span data-stu-id="4cc41-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="4cc41-109">Windows essaiera de réinstaller le pilote.</span><span class="sxs-lookup"><span data-stu-id="4cc41-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="4cc41-110">Si vous avez récemment installé les mises à jour de Windows 10 ou mis à niveau vers Windows 10, vous souhaiterez peut-être vérifier les mises à jour de pilotes :</span><span class="sxs-lookup"><span data-stu-id="4cc41-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="4cc41-111">Dans le gestionnaire de périphériques, cliquez sur **Bluetooth**, puis sur le nom de la carte Bluetooth (qui peut inclure le mot « radio »).</span><span class="sxs-lookup"><span data-stu-id="4cc41-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="4cc41-112">Appuyez longuement (ou cliquez avec le bouton droit) sur la carte Bluetooth, puis cliquez sur **mettre à jour**la  >  **recherche de pilote automatiquement pour le logiciel de pilote mis à jour**.</span><span class="sxs-lookup"><span data-stu-id="4cc41-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="4cc41-113">Suivez les étapes, puis cliquez sur **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="4cc41-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="4cc41-114">Si Windows ne trouve pas de nouveau pilote Bluetooth, visitez le site Web du fabricant de PC et téléchargez le pilote Bluetooth le plus récent à partir de là.</span><span class="sxs-lookup"><span data-stu-id="4cc41-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="4cc41-115">Une fois le téléchargement effectué, cliquez sur **mettre à jour le pilote**parcourir le lecteur  >  **mon ordinateur pour le pilote logiciel**  >  **recherchez** l’emplacement où sont stockés les fichiers du pilote > **OK**  >  **Next**, puis suivez les étapes d’installation.</span><span class="sxs-lookup"><span data-stu-id="4cc41-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="4cc41-116">Après avoir installé le pilote mis à jour, redémarrez l’ordinateur, puis vérifiez si cela résout le problème de connexion.</span><span class="sxs-lookup"><span data-stu-id="4cc41-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="4cc41-117">Pour plus d’informations sur la résolution des problèmes liés à Bluetooth, reportez-vous à l’article complet relatif à la [résolution des problèmes Bluetooth dans Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="4cc41-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
