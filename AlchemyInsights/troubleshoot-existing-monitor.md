---
title: Résolution des problèmes de moniteur existant
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690709"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="b9d54-102">Résoudre les problèmes d’un moniteur existant</span><span class="sxs-lookup"><span data-stu-id="b9d54-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="b9d54-103">Essayez ces solutions pour dépanner un moniteur.</span><span class="sxs-lookup"><span data-stu-id="b9d54-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="b9d54-104">**Actualisez l’affichage de votre moniteur :**</span><span class="sxs-lookup"><span data-stu-id="b9d54-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="b9d54-105">Appuyez simultanément sur les touches suivantes : touche Windows + Ctrl + Maj + B. Cette opération permet d’actualiser la communication avec votre pilote graphique.</span><span class="sxs-lookup"><span data-stu-id="b9d54-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="b9d54-106">Vos moniteurs clignotent momentanément et reviennent après quelques secondes.</span><span class="sxs-lookup"><span data-stu-id="b9d54-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="b9d54-107">**Dépanner le matériel de surveillance :**</span><span class="sxs-lookup"><span data-stu-id="b9d54-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="b9d54-108">Débranchez le câble reliant votre PC à votre moniteur, puis reconnectez-le.</span><span class="sxs-lookup"><span data-stu-id="b9d54-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="b9d54-109">Déconnectez les appareils non essentiels de votre PC (cartes ou stations d’accueil, par exemple).</span><span class="sxs-lookup"><span data-stu-id="b9d54-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="b9d54-110">**Si vous avez récemment installé une mise à jour sur votre PC, vous pouvez restaurer votre pilote d’affichage :**</span><span class="sxs-lookup"><span data-stu-id="b9d54-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="b9d54-111">Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans les résultats.</span><span class="sxs-lookup"><span data-stu-id="b9d54-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="b9d54-112">Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte vidéo, opérateurs and sélectionnez **Propriétés**.</span><span class="sxs-lookup"><span data-stu-id="b9d54-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="b9d54-113">Accédez à l’onglet **pilote** et sélectionnez **restaurer le pilote**.</span><span class="sxs-lookup"><span data-stu-id="b9d54-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="b9d54-114">Remarque : si cette option n’est pas disponible ou est grisée, sélectionnez **non** parmi les options ci-dessous pour passer à l’étape suivante.</span><span class="sxs-lookup"><span data-stu-id="b9d54-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="b9d54-115">Vous devrez peut-être redémarrer votre PC pour que ces modifications prennent effet.</span><span class="sxs-lookup"><span data-stu-id="b9d54-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="b9d54-116">**Désinstallez et réinstallez votre pilote d’affichage :**</span><span class="sxs-lookup"><span data-stu-id="b9d54-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="b9d54-117">Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans les résultats.</span><span class="sxs-lookup"><span data-stu-id="b9d54-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="b9d54-118">Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte vidéo, opérateurs and sélectionnez **désinstaller le périphérique**.</span><span class="sxs-lookup"><span data-stu-id="b9d54-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="b9d54-119">Activez la case à cocher en regard de **supprimer le pilote logiciel de ce périphérique** , puis sélectionnez **désinstaller**.</span><span class="sxs-lookup"><span data-stu-id="b9d54-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="b9d54-120">Remarque : vous serez peut-être invité à redémarrer votre ordinateur à ce stade.</span><span class="sxs-lookup"><span data-stu-id="b9d54-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="b9d54-121">Veillez à noter les autres instructions avant de redémarrer.</span><span class="sxs-lookup"><span data-stu-id="b9d54-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="b9d54-122">Ouvrez à nouveau le gestionnaire de périphériques.</span><span class="sxs-lookup"><span data-stu-id="b9d54-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="b9d54-123">Développez la section **cartes graphiques** , cliquez avec le bouton droit sur votre carte graphique, puis sélectionnez **mettre à jour le pilote**.</span><span class="sxs-lookup"><span data-stu-id="b9d54-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="b9d54-124">Sélectionnez **recherche automatique pour mettre à jour le pilote logiciel** et suivez les instructions d’installation.</span><span class="sxs-lookup"><span data-stu-id="b9d54-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>