---
title: Utiliser l’option de déverrouillage d’empreinte digitale dans Windows 10
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
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971901"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Utiliser l’option de déverrouillage d’empreinte digitale dans Windows 10

**Activer Windows Hello empreinte digitale**

Pour déverrouiller Windows 10 l’aide de votre empreinte digitale, vous devez configurer Windows Hello empreinte digitale en ajoutant (permettant Windows apprendre à reconnaître) au moins un doigt. 

1. Go to **Paramètres > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)). Les options de personnalisation disponibles sont répertoriées. Par exemple :

    ![Options de connectez-vous.](media/sign-in-options.png)

2. Cliquez ou appuyez **Windows Hello empreinte** digitale, puis cliquez **sur Configurer.** Dans la Windows Hello d’installation, cliquez **sur Démarrer.** Le capteur d’empreintes digitales s’active et vous êtes invité à placer votre doigt sur le capteur :

   ![Capteur d’empreintes digitales.](media/fingerprint-sensor.png)

3. Suivez les instructions qui vous demanderont d’analyser votre doigt à plusieurs reprises. Lorsque cette option est terminée, vous avez la possibilité d’ajouter d’autres doigts que vous souhaiterez peut-être utiliser pour vous inscrire. La prochaine fois que vous vous connectez Windows 10, vous aurez la possibilité d’utiliser votre empreinte digitale pour le faire.

**Windows Hello Empreinte digitale non disponible en tant qu’option de sign-in**

Si Windows Hello Fingerprint n’est pas affiché en tant qu’option dans les **options** de signature, cela signifie que Windows ne connaît aucun lecteur/scanneur d’empreintes digitales connecté à votre PC, ou qu’une stratégie système empêche son utilisation (si, par exemple, votre PC est géré par votre espace de travail). Pour résoudre les problèmes : 

1. Sélectionnez **le bouton** Démarrer dans la barre des tâches et recherchez Gestionnaire de **périphériques.**

2. Cliquez ou appuyez pour ouvrir **le Gestionnaire de périphériques.**

3. Dans le Gestionnaire de périphériques, développez les appareils biométriques en cliquant sur son chevron.

   ![Appareils biométriques.](media/biometric-devices.png)

4. Votre scanneur d’empreintes digitales doit être répertorié en tant que périphérique biométrique, tel que le scanneur Synaptics WBDI :

   ![Appareils biométriques.](media/biometric-devices-expanded.png)

5. Si votre scanneur d’empreintes digitales n’est pas affiché et qu’il est intégré à votre PC, allez sur le site web du fabricant du PC. Dans la section de support technique pour votre modèle de PC, recherchez un pilote Windows 10 pour un scanneur que vous pouvez installer.

6. Si le scanneur est distinct du PC (connecté via USB), allez sur le site web du fabricant du scanneur pour rechercher et installer le logiciel de pilote de périphérique Windows 10 pour le modèle de scanneur dont vous avez besoin.
