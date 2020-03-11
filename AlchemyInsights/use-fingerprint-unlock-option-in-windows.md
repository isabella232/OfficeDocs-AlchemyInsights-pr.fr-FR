---
title: Utiliser l’option de déverrouillage par empreinte digitale dans Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588314"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="12d96-102">Utiliser l’option de déverrouillage par empreinte digitale dans Windows 10</span><span class="sxs-lookup"><span data-stu-id="12d96-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="12d96-103">**Activer l’empreinte digitale Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="12d96-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="12d96-104">Pour déverrouiller Windows 10 à l’aide de votre empreinte digitale, vous devez configurer une empreinte digitale Windows Hello en ajoutant (permettant à Windows d’apprendre à reconnaître) au moins un doigt.</span><span class="sxs-lookup"><span data-stu-id="12d96-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="12d96-105">Accédez à **paramètres > comptes > options de connexion** (ou cliquez sur [ici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="12d96-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="12d96-106">Les options de connexion disponibles seront affichées.</span><span class="sxs-lookup"><span data-stu-id="12d96-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="12d96-107">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="12d96-107">For example:</span></span>

    ![Options de connexion.](media/sign-in-options.png)

2. <span data-ttu-id="12d96-109">Cliquez ou appuyez sur **Windows Hello Fingerprint**, puis cliquez sur **configurer**.</span><span class="sxs-lookup"><span data-stu-id="12d96-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="12d96-110">Dans la fenêtre installation de Windows Hello, cliquez sur **prise en main**.</span><span class="sxs-lookup"><span data-stu-id="12d96-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="12d96-111">Le capteur d’empreintes digitales est activé et vous êtes invité à placer votre doigt sur le capteur :</span><span class="sxs-lookup"><span data-stu-id="12d96-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Capteur d’empreintes digitales.](media/fingerprint-sensor.png)

3. <span data-ttu-id="12d96-113">Suivez les instructions, qui vous demanderont d’analyser votre doigt de manière répétée.</span><span class="sxs-lookup"><span data-stu-id="12d96-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="12d96-114">Une fois cette opération terminée, vous aurez la possibilité d’ajouter d’autres doigts que vous souhaiterez peut-être utiliser pour vous connecter.</span><span class="sxs-lookup"><span data-stu-id="12d96-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="12d96-115">La prochaine fois que vous vous connecterez à Windows 10, vous aurez la possibilité d’utiliser votre empreinte digitale pour le faire.</span><span class="sxs-lookup"><span data-stu-id="12d96-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="12d96-116">**Empreinte digitale Windows Hello non disponible en tant qu’option de connexion**</span><span class="sxs-lookup"><span data-stu-id="12d96-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="12d96-117">Si Windows Hello Fingerprint n’est pas affiché en tant qu’option dans les **options de connexion**, cela signifie que Windows n’est pas conscient d’un lecteur d’empreintes digitales ou d’un scanneur connecté à votre PC, ou qu’une stratégie système empêche son utilisation (si votre PC est géré par exemple).</span><span class="sxs-lookup"><span data-stu-id="12d96-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="12d96-118">Pour résoudre les problèmes :</span><span class="sxs-lookup"><span data-stu-id="12d96-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="12d96-119">Sélectionnez le bouton **Démarrer** dans la barre des tâches et recherchez **Gestionnaire de périphériques**.</span><span class="sxs-lookup"><span data-stu-id="12d96-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="12d96-120">Cliquez ou appuyez pour ouvrir le **Gestionnaire de périphériques**.</span><span class="sxs-lookup"><span data-stu-id="12d96-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="12d96-121">Dans le gestionnaire de périphériques, développez périphériques biométriques en cliquant sur le Chevron correspondant.</span><span class="sxs-lookup"><span data-stu-id="12d96-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Périphériques biométriques.](media/biometric-devices.png)

4. <span data-ttu-id="12d96-123">Votre scanneur d’empreintes digitales doit être mentionné comme un périphérique biométrique, tel que le scanneur Synaptics WBDI :</span><span class="sxs-lookup"><span data-stu-id="12d96-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Périphériques biométriques.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="12d96-125">Si votre scanneur d’empreintes digitales n’est pas affiché et que le scanneur est intégré à votre PC, accédez au site Web du fabricant de PC.</span><span class="sxs-lookup"><span data-stu-id="12d96-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="12d96-126">Dans la section Support technique de votre modèle PC, recherchez un pilote Windows 10 pour un scanneur que vous pouvez installer.</span><span class="sxs-lookup"><span data-stu-id="12d96-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="12d96-127">Si le scanneur est séparé du PC (attaché via USB), accédez au site Web du fabricant du scanneur pour trouver et installer le logiciel de pilote de périphérique Windows 10 pour le modèle de scanneur que vous avez.</span><span class="sxs-lookup"><span data-stu-id="12d96-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
