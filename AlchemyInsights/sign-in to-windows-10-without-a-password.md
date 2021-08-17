---
title: Connectez-vous à Windows 10 sans utiliser de mot de passe
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107506"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Connectez-vous à Windows 10 sans utiliser de mot de passe

Pour éviter d’avoir à taper un mot de passe au démarrage de Windows, nous vous recommandons d’utiliser l’une des options de Windows Hello de signature sécurisée, comme un code confidentiel, une reconnaissance faciale ou une empreinte digitale, si disponible. Si vous souhaitez vraiment désactiver la sign-in sécurisée, consultez les instructions « Se Windows 10 » ci-dessous.

**Options de Windows Hello de sécurité au mot de passe du compte**

Go to **Paramètres > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)). Les options de personnalisation disponibles sont répertoriées. Par exemple :

![Options de connectez-vous.](media/sign-in-options.png)

Cliquez ou appuyez sur l’une des options pour la configurer. La prochaine fois que vous démarrerez ou déverrouillez Windows, vous pourrez utiliser la nouvelle option au lieu d’un mot de passe. 

**Connectez-vous automatiquement à Windows 10**

**Remarque**: la connectez-vous automatique est pratique, mais présente un risque de sécurité, en particulier si votre PC est accessible par plusieurs personnes. 

1. Cliquez ou appuyez sur **le bouton** Démarrer dans la barre des tâches.

2. Tapez **netplwiz** et touchez la touche Entrée pour ouvrir la fenêtre Comptes d’utilisateurs.

3. Dans **Comptes d’utilisateurs,** cliquez sur le compte à qui vous souhaitez vous Windows automatiquement.

4. Décochez la case « Les utilisateurs doivent entrer un nom d’utilisateur et un mot de passe pour utiliser cet ordinateur ».

    ![Les utilisateurs doivent entrer un nom d’utilisateur et une option de mot de passe.](media/users-must-enter-username.png)

5. Cliquez sur **OK**. Vous serez invité à entrer et à confirmer le mot de passe du compte que vous avez sélectionné. Cliquez sur **OK** pour terminer. La prochaine fois Windows 10, il se connecte automatiquement au compte que vous avez sélectionné.
