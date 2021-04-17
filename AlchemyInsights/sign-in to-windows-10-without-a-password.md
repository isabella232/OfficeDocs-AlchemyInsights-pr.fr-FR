---
title: Se connectez à Windows 10 sans utiliser de mot de passe
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
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830544"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Se connectez à Windows 10 sans utiliser de mot de passe

Pour éviter d'avoir à taper un mot de passe au démarrage de Windows, nous vous recommandons d'utiliser l'une des options de connectez-vous sécurisé Windows Hello, comme un code confidentiel, une reconnaissance faciale ou une empreinte digitale, si disponible. Si vous souhaitez vraiment désactiver la sign-in sécurisée, consultez les instructions « Se connectez automatiquement à Windows 10 » ci-dessous.

**Autres solutions Windows Hello sécurisées que le mot de passe du compte**

Go to **Settings > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)). Les options de personnalisation disponibles sont répertoriées. Par exemple :

![Options de connectez-vous.](media/sign-in-options.png)

Cliquez ou appuyez sur l'une des options pour la configurer. La prochaine fois que vous démarrerez ou déverrouillez Windows, vous pourrez utiliser la nouvelle option au lieu d'un mot de passe. 

**Se connectez automatiquement à Windows 10**

**Remarque**: la connectez-vous automatique est pratique, mais présente un risque de sécurité, en particulier si votre PC est accessible par plusieurs personnes. 

1. Cliquez ou appuyez sur **le bouton** Démarrer dans la barre des tâches.

2. Tapez **netplwiz** et touchez la touche Entrée pour ouvrir la fenêtre Comptes d'utilisateurs.

3. Dans **Comptes d'utilisateurs,** cliquez sur le compte à qui vous souhaitez vous inscrire automatiquement au démarrage de Windows.

4. Décochez la case « Les utilisateurs doivent entrer un nom d'utilisateur et un mot de passe pour utiliser cet ordinateur ».

    ![Les utilisateurs doivent entrer un nom d'utilisateur et une option de mot de passe.](media/users-must-enter-username.png)

5. Cliquez sur **OK**. Vous serez invité à entrer et à confirmer le mot de passe du compte que vous avez sélectionné. Cliquez sur **OK** pour terminer. La prochaine fois que Windows 10 démarre, il se connecte automatiquement au compte que vous avez sélectionné.
