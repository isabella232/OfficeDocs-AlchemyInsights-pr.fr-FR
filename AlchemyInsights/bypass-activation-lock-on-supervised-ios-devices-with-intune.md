---
title: Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397731"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="4b487-102">Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune</span><span class="sxs-lookup"><span data-stu-id="4b487-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="4b487-103">La possibilité de contourner le verrou d’activation sur les appareils iOS simplifie la récupération du scénario dans lequel un utilisateur active le verrouillage d’activation sur un appareil d’entreprise, puis quitte l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="4b487-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="4b487-104">Les conditions préalables au contournement d'un verrou d'activation sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="4b487-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="4b487-105">Un appareil est « supervisé ».</span><span class="sxs-lookup"><span data-stu-id="4b487-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="4b487-106">Le verrou d’activation est correctement activé à l’aide de la stratégie de restriction des appareils iOS dans Intune.</span><span class="sxs-lookup"><span data-stu-id="4b487-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="4b487-107">En outre, lorsque vous contournez un verrou d'activation, vous devez :</span><span class="sxs-lookup"><span data-stu-id="4b487-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="4b487-108">Posséder physiquement l'appareil à nettoyer.</span><span class="sxs-lookup"><span data-stu-id="4b487-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="4b487-109">Copier le code avant de lancer la réinitialisation.</span><span class="sxs-lookup"><span data-stu-id="4b487-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="4b487-110">**Remarque :** le code de réinitialisation ne respecte pas la casse. par conséquent, les caractères « - » ne sont pas obligatoires.</span><span class="sxs-lookup"><span data-stu-id="4b487-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="4b487-111">Pour plus d’informations, consultez [Contourner le verrou d’activation sur les appareils iOS supervisés avec Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="4b487-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="4b487-112">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="4b487-112">**FAQ**</span></span>

<span data-ttu-id="4b487-113">Q : **j'ai lancé une action à distance pour supprimer les données de l'entreprise d'un appareil, et l'état d'attente est maintenant bloqué.**</span><span class="sxs-lookup"><span data-stu-id="4b487-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="4b487-114">R : pour qu'une action à distance soit menée à bien, l'appareil ciblé doit être en ligne et sain.</span><span class="sxs-lookup"><span data-stu-id="4b487-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="4b487-115">Dans les situations suivantes, l’action distante reste dans un état d’attente pendant 30 jours, ou jusqu’à ce que l’appareil accuse la commande lorsque l’appareil :</span><span class="sxs-lookup"><span data-stu-id="4b487-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="4b487-116">Ne possède pas de connectivité.</span><span class="sxs-lookup"><span data-stu-id="4b487-116">Does not have connectivity.</span></span>
- <span data-ttu-id="4b487-117">Perd son statut de gestion avec Intune.</span><span class="sxs-lookup"><span data-stu-id="4b487-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="4b487-118">Si vous pensez qu'un appareil n'est plus enregistré, et qu'il ne supprime pas les données de l'entreprise, sélectionnez Supprimer.</span><span class="sxs-lookup"><span data-stu-id="4b487-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="4b487-119">La suppression supprime l'enregistrement de l'appareil afin qu'il n'apparaisse plus dans la liste des appareils d'Intune.</span><span class="sxs-lookup"><span data-stu-id="4b487-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="4b487-120">Pour que l'appareil redevienne actif, son utilisateur doit le réinscrire.</span><span class="sxs-lookup"><span data-stu-id="4b487-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="4b487-121">Q : **pourquoi certaines actions à distance ne sont-elles pas disponibles pour mon utilisation ?**</span><span class="sxs-lookup"><span data-stu-id="4b487-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="4b487-122">R : toutes les plateformes ne prennent pas en charge toutes les actions de périphériques distants.</span><span class="sxs-lookup"><span data-stu-id="4b487-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="4b487-123">Les actions distantes suivantes sont spécifiques aux plateformes.</span><span class="sxs-lookup"><span data-stu-id="4b487-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="4b487-124">Contourner le verrou d’activation (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="4b487-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="4b487-125">Nouveau démarrage (Windows uniquement)</span><span class="sxs-lookup"><span data-stu-id="4b487-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="4b487-126">Mode perdu (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="4b487-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="4b487-127">Localiser l’appareil (iOS uniquement)</span><span class="sxs-lookup"><span data-stu-id="4b487-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="4b487-128">Redémarrer (Windows uniquement)</span><span class="sxs-lookup"><span data-stu-id="4b487-128">Restart (Windows only)</span></span>

<span data-ttu-id="4b487-129">Pour plus d’informations sur chaque action, consultez [Actions d’appareil disponibles](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="4b487-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>