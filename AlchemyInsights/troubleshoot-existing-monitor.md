---
title: Résolution des problèmes d'un moniteur existant
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824577"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="9d7a7-102">Résoudre les problèmes d'un moniteur existant</span><span class="sxs-lookup"><span data-stu-id="9d7a7-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="9d7a7-103">Essayez ces solutions pour résoudre les problèmes d'un moniteur.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="9d7a7-104">**Actualisez l'affichage de votre moniteur :**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="9d7a7-105">Appuyez sur les touches suivantes en même temps : Touche Windows + Ctrl + Décalage + B. Cela permettra d'actualiser la communication avec votre pilote graphique.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="9d7a7-106">Vos moniteurs clignotent momentanément et reviennent après quelques secondes.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="9d7a7-107">**Résoudre les problèmes de matériel du moniteur :**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="9d7a7-108">Débranchez le câble qui connecte votre PC à votre moniteur, puis branchez-le à nouveau.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="9d7a7-109">Déconnectez les appareils non essentiels de votre PC (par exemple, les cartes ou les docks).</span><span class="sxs-lookup"><span data-stu-id="9d7a7-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="9d7a7-110">**Si vous avez récemment installé une mise à jour sur votre PC, vous pouvez revenir en arrière de votre pilote d'affichage :**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="9d7a7-111">Sélectionnez **Démarrer,** **tapez gestionnaire de** périphériques et sélectionnez **Gestionnaire de périphériques** dans les résultats.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="9d7a7-112">Développez la section **Cartes d'affichage,** cliquez avec le bouton droit sur votre carte d'affichage et sélectionnez **Propriétés.**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="9d7a7-113">Accédez à **l'onglet Pilote** et **sélectionnez Revenir en arrière.**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="9d7a7-114">Remarque : si cette option n'est pas  disponible ou est grisée, sélectionnez Non dans les options ci-dessous pour passer à l'étape suivante.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="9d7a7-115">Vous devrez peut-être redémarrer votre PC avant que ces modifications prennent effet.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="9d7a7-116">**Désinstallez et réinstallez votre pilote d'affichage :**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="9d7a7-117">Sélectionnez **Démarrer,** **tapez gestionnaire de** périphériques et sélectionnez **Gestionnaire de périphériques** dans les résultats.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="9d7a7-118">Développez la section **Cartes d'affichage,** cliquez avec le bouton droit sur votre carte d'affichage, puis **sélectionnez Désinstaller l'appareil.**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="9d7a7-119">Sélectionnez la case à côté **de Supprimer le logiciel de pilote pour cet appareil,** puis **sélectionnez Désinstaller.**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="9d7a7-120">Remarque : vous pouvez être invité à redémarrer votre ordinateur à ce stade.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="9d7a7-121">Veillez à noter les instructions restantes avant de redémarrer.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="9d7a7-122">Ouvrez de nouveau le Gestionnaire de périphériques.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="9d7a7-123">Développez la section **Cartes d'affichage,** cliquez avec le bouton droit sur votre carte d'affichage, puis sélectionnez Mettre à **jour le pilote.**</span><span class="sxs-lookup"><span data-stu-id="9d7a7-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="9d7a7-124">Sélectionnez **Rechercher automatiquement pour le logiciel du pilote de mise à** jour et suivez les instructions d'installation.</span><span class="sxs-lookup"><span data-stu-id="9d7a7-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>