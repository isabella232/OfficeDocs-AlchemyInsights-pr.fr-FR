---
title: Localisation de pertes d’appareils iOS avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675157"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="c4861-102">Localisation de pertes d’appareils iOS avec Intune</span><span class="sxs-lookup"><span data-stu-id="c4861-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="c4861-103">L’activation du mode perdu sur un appareil iOS permet à un administrateur d’avoir un message et un numéro de téléphone de contact affichés sur l’écran de verrouillage.</span><span class="sxs-lookup"><span data-stu-id="c4861-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="c4861-104">Une fois le mode perdu activé, l’administrateur peut utiliser l’action localiser l’appareil pour identifier l’emplacement physique de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="c4861-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="c4861-105">L’action localiser l’appareil dans Intune fonctionne avec les appareils iOS pour afficher l’emplacement d’un appareil spécifique sur une carte.</span><span class="sxs-lookup"><span data-stu-id="c4861-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="c4861-106">L’utilisation de cette action nécessite que l’appareil iOS soit en :</span><span class="sxs-lookup"><span data-stu-id="c4861-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="c4861-107">Mode supervisé</span><span class="sxs-lookup"><span data-stu-id="c4861-107">Supervised mode</span></span>
- <span data-ttu-id="c4861-108">Mode Perdu</span><span class="sxs-lookup"><span data-stu-id="c4861-108">Lost mode</span></span>

<span data-ttu-id="c4861-109">Pour plus d’informations, consultez [Activer le mode perdu sur les appareils iOS/iPad avec Intune](https://docs.microsoft.com/intune/device-lost-mode) et [Localiser les appareils iOS/iPad d’iOS perdus ou volés avec Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="c4861-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="c4861-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="c4861-110">**FAQ**</span></span>

<span data-ttu-id="c4861-111">Q : j'ai lancé une action à distance pour supprimer les données de l'entreprise d'un appareil, et l'état d'attente est maintenant bloqué.</span><span class="sxs-lookup"><span data-stu-id="c4861-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="c4861-112">R : pour qu'une action à distance soit menée à bien, l'appareil ciblé doit être en ligne et sain.</span><span class="sxs-lookup"><span data-stu-id="c4861-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="c4861-113">Dans les situations suivantes, l’action distante reste dans un état d’attente pendant 30 jours, ou jusqu’à ce que l’appareil accuse la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="c4861-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="c4861-114">Lorsque l’appareil ne possède pas de connectivité</span><span class="sxs-lookup"><span data-stu-id="c4861-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="c4861-115">Lorsque l’appareil perd son état de gestion avec Intune</span><span class="sxs-lookup"><span data-stu-id="c4861-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="c4861-116">Si vous pensez qu'un appareil n'est plus enregistré, et qu'il ne peut pas supprime les données de l'entreprise, sélectionnez Supprimer.</span><span class="sxs-lookup"><span data-stu-id="c4861-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="c4861-117">La suppression supprime l'enregistrement de l'appareil afin qu'il n'apparaisse plus dans la liste des appareils d'Intune.</span><span class="sxs-lookup"><span data-stu-id="c4861-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="c4861-118">Si l’appareil redevient actif, l’utilisateur doit le ré-inscrire.</span><span class="sxs-lookup"><span data-stu-id="c4861-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="c4861-119">Q : pourquoi certaines actions à distance ne sont-elles pas disponibles pour mon utilisation ?</span><span class="sxs-lookup"><span data-stu-id="c4861-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="c4861-120">R : toutes les plateformes ne prennent pas en charge toutes les actions de périphériques distants.</span><span class="sxs-lookup"><span data-stu-id="c4861-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="c4861-121">Les actions distantes suivantes sont spécifiques aux plateformes, de sorte qu’elles sont disponibles uniquement pour les plateformes indiquées.</span><span class="sxs-lookup"><span data-stu-id="c4861-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="c4861-122">Contourner le verrou d’activation (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="c4861-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="c4861-123">Nouveau démarrage (Windows uniquement)</span><span class="sxs-lookup"><span data-stu-id="c4861-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="c4861-124">Mode perdu (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="c4861-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="c4861-125">Localiser l’appareil (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="c4861-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="c4861-126">Redémarrer (Windows uniquement)</span><span class="sxs-lookup"><span data-stu-id="c4861-126">Restart (Windows only)</span></span>

<span data-ttu-id="c4861-127">Pour plus d’informations sur chaque action, consultez [Actions d’appareil disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="c4861-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>