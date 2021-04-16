---
title: Utiliser l'option de déverrouillage d'empreinte digitale dans Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796675"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="695b1-102">Utiliser l'option de déverrouillage d'empreinte digitale dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="695b1-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="695b1-103">**Activer l'empreinte numérique Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="695b1-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="695b1-104">Pour déverrouiller Windows 10 à l'aide de votre empreinte digitale, vous devez configurer l'empreinte digitale Windows Hello en ajoutant (permettant à Windows d'apprendre à reconnaître) au moins un doigt.</span><span class="sxs-lookup"><span data-stu-id="695b1-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="695b1-105">Go to **Settings > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="695b1-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="695b1-106">Les options de personnalisation disponibles sont répertoriées.</span><span class="sxs-lookup"><span data-stu-id="695b1-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="695b1-107">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="695b1-107">For example:</span></span>

    ![Options de connectez-vous.](media/sign-in-options.png)

2. <span data-ttu-id="695b1-109">Cliquez ou appuyez **sur Windows Hello Fingerprint,** puis cliquez **sur Configurer**.</span><span class="sxs-lookup"><span data-stu-id="695b1-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="695b1-110">Dans la fenêtre d'installation de Windows Hello, cliquez **sur Démarrer.**</span><span class="sxs-lookup"><span data-stu-id="695b1-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="695b1-111">Le capteur d'empreintes digitales s'active et vous êtes invité à placer votre doigt sur le capteur :</span><span class="sxs-lookup"><span data-stu-id="695b1-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Capteur d'empreintes digitales.](media/fingerprint-sensor.png)

3. <span data-ttu-id="695b1-113">Suivez les instructions qui vous demanderont d'analyser votre doigt à plusieurs reprises.</span><span class="sxs-lookup"><span data-stu-id="695b1-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="695b1-114">Lorsque cette option est terminée, vous avez la possibilité d'ajouter d'autres doigts que vous souhaiterez peut-être utiliser pour vous inscrire.</span><span class="sxs-lookup"><span data-stu-id="695b1-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="695b1-115">La prochaine fois que vous vous connectez à Windows 10, vous aurez la possibilité d'utiliser votre empreinte digitale pour le faire.</span><span class="sxs-lookup"><span data-stu-id="695b1-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="695b1-116">**Windows Hello Fingerprint non disponible en tant qu'option de sign-in**</span><span class="sxs-lookup"><span data-stu-id="695b1-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="695b1-117">Si l'empreinte digitale Windows Hello n'est pas affichée en tant qu'option dans les **options** de personnalisation, cela signifie que Windows ne connaît aucun lecteur/scanneur d'empreintes digitales connecté à votre PC, ou qu'une stratégie système empêche son utilisation (si, par exemple, votre PC est géré par votre espace de travail).</span><span class="sxs-lookup"><span data-stu-id="695b1-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="695b1-118">Pour résoudre les problèmes :</span><span class="sxs-lookup"><span data-stu-id="695b1-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="695b1-119">Sélectionnez **le bouton** Démarrer dans la barre des tâches et recherchez Gestionnaire de **périphériques.**</span><span class="sxs-lookup"><span data-stu-id="695b1-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="695b1-120">Cliquez ou appuyez pour ouvrir **le Gestionnaire de périphériques.**</span><span class="sxs-lookup"><span data-stu-id="695b1-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="695b1-121">Dans le Gestionnaire de périphériques, développez les appareils biométriques en cliquant sur son chevron.</span><span class="sxs-lookup"><span data-stu-id="695b1-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Appareils biométriques.](media/biometric-devices.png)

4. <span data-ttu-id="695b1-123">Votre scanneur d’empreintes digitales doit être répertorié en tant que périphérique biométrique, tel que le scanneur Synaptics WBDI :</span><span class="sxs-lookup"><span data-stu-id="695b1-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Appareils biométriques.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="695b1-125">Si votre scanneur d’empreintes digitales n’est pas affiché et qu’il est intégré à votre PC, allez sur le site web du fabricant du PC.</span><span class="sxs-lookup"><span data-stu-id="695b1-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="695b1-126">Dans la section de support technique de votre modèle PC, recherchez un pilote Windows 10 pour un scanneur que vous pouvez installer.</span><span class="sxs-lookup"><span data-stu-id="695b1-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="695b1-127">Si le scanneur est distinct du PC (connecté via USB), allez sur le site web du fabricant du scanneur pour rechercher et installer le logiciel de pilote de périphérique Windows 10 pour le modèle de scanneur dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="695b1-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
