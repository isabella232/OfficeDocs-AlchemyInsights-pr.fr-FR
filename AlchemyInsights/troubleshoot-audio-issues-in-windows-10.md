---
title: Résoudre les problèmes audio dans Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796107"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="4e860-102">Résolution des problèmes audio dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="4e860-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="4e860-103">**Exécuter l’utilitaire de résolution des problèmes audio**</span><span class="sxs-lookup"><span data-stu-id="4e860-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="4e860-104">L’utilitaire de résolution des problèmes audio peut résoudre automatiquement les problèmes audio :</span><span class="sxs-lookup"><span data-stu-id="4e860-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="4e860-105">Sélectionnez **Démarrer**, tapez **dépanner**, puis sélectionnez **résolution des problèmes** dans la liste des résultats.</span><span class="sxs-lookup"><span data-stu-id="4e860-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="4e860-106">Sélectionnez **lecture audio** > **Exécutez l’utilitaire de résolution des problèmes**.</span><span class="sxs-lookup"><span data-stu-id="4e860-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="4e860-107">**Vérifier les câbles, le volume, les haut-parleurs et le casque**</span><span class="sxs-lookup"><span data-stu-id="4e860-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="4e860-108">Vérifiez que les câbles de votre haut-parleur et de votre casque sont connectés et assurez-vous qu’ils sont connectés à la bonne prise.</span><span class="sxs-lookup"><span data-stu-id="4e860-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="4e860-109">Vérifiez les niveaux de puissance et de volume, puis essayez de relancer tous les contrôles de volume.</span><span class="sxs-lookup"><span data-stu-id="4e860-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="4e860-110">Certains haut-parleurs et applications ont leurs propres contrôles de volume, et vous devrez peut-être les vérifier tous pour vous assurer qu’ils sont aux niveaux corrects.</span><span class="sxs-lookup"><span data-stu-id="4e860-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="4e860-111">Essayez de vous connecter à l’aide d’un autre port USB.</span><span class="sxs-lookup"><span data-stu-id="4e860-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="4e860-112">**Remarque :** N’oubliez pas que vos haut-parleurs ne fonctionnent pas lorsque le casque est branché.</span><span class="sxs-lookup"><span data-stu-id="4e860-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="4e860-113">**Vérifier le gestionnaire de périphériques**</span><span class="sxs-lookup"><span data-stu-id="4e860-113">**Check Device Manager**</span></span>

<span data-ttu-id="4e860-114">Pour vous assurer que les pilotes sont à jour :</span><span class="sxs-lookup"><span data-stu-id="4e860-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="4e860-115">Sélectionnez **Démarrer**, tapez **Gestionnaire de périphériques**, puis sélectionnez **Gestionnaire de périphériques** dans la liste des résultats.</span><span class="sxs-lookup"><span data-stu-id="4e860-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="4e860-116">Sous **Contrôleurs audio, vidéo et jeu**, sélectionnez votre carte audio, ouvrez-la, sélectionnez l’onglet **pilote** , puis sélectionnez **mettre à jour le pilote**.</span><span class="sxs-lookup"><span data-stu-id="4e860-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="4e860-117">**Remarque :** Si Windows ne trouve pas de nouveau pilote, recherchez-en un sur le site Web du fabricant de l’appareil et suivez les instructions.</span><span class="sxs-lookup"><span data-stu-id="4e860-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="4e860-118">**Réinstaller le pilote**</span><span class="sxs-lookup"><span data-stu-id="4e860-118">**Reinstall the driver**</span></span>

<span data-ttu-id="4e860-119">Si vous ne pouvez pas effectuer une mise à jour via le gestionnaire de périphériques ou si vous recherchez un nouveau pilote sur le site Web du fabricant, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="4e860-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="4e860-120">Dans le gestionnaire de périphériques, cliquez avec le bouton droit (ou appuyez longuement) sur le pilote audio, puis sélectionnez **désinstaller**.</span><span class="sxs-lookup"><span data-stu-id="4e860-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="4e860-121">Redémarrez votre appareil et Windows tentera de réinstaller le pilote.</span><span class="sxs-lookup"><span data-stu-id="4e860-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="4e860-122">Si la réinstallation du pilote ne fonctionne pas, essayez d’utiliser le pilote audio générique fourni avec Windows.</span><span class="sxs-lookup"><span data-stu-id="4e860-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="4e860-123">Dans le gestionnaire de périphériques, cliquez avec le bouton droit de la touche (ou appuyez longuement) sur votre pilote audio > **mettre à jour le logiciel** > **de pilote pour rechercher le pilote logiciel** > , sélectionnez l'**une des pilotes de périphériques sur mon ordinateur**, sélectionnez **périphérique audio haute définition**, sélectionnez **suivant**, puis suivez les instructions pour l’installer.</span><span class="sxs-lookup"><span data-stu-id="4e860-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="4e860-124">**Définir le périphérique par défaut**</span><span class="sxs-lookup"><span data-stu-id="4e860-124">**Set the default device**</span></span>

<span data-ttu-id="4e860-125">Si vous vous connectez à un périphérique audio à l’aide de l’USB ou de l’HDMI, vous devrez peut-être définir ce périphérique par défaut :</span><span class="sxs-lookup"><span data-stu-id="4e860-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="4e860-126">Sélectionnez **Démarrer**, tapez **son**, puis sélectionnez **son** ou **Modifiez sons système** dans la liste des résultats.</span><span class="sxs-lookup"><span data-stu-id="4e860-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="4e860-127">Sous l’onglet **lecture** , sélectionnez un appareil, sélectionnez **définir la valeur par défaut**, puis **OK**.</span><span class="sxs-lookup"><span data-stu-id="4e860-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

