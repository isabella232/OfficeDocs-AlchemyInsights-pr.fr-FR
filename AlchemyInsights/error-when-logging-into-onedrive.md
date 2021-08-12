---
title: 0x8004de40'erreur lors du lancement OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946577"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40'erreur lors du lancement OneDrive

Si vous recevez un message **d'0x8004de40** lors de la connexion à OneDrive, redémarrez l’ordinateur lorsque vous êtes connecté à votre domaine scolaire ou scolaire. Si vous recevez cette erreur après le redémarrage, essayez ceci lorsque vous êtes connecté à votre domaine scolaire ou scolaire :

1. Cliquez sur Démarrer, puis tapez **cmd** **ou** invite de commandes dans la zone de recherche, cliquez avec le bouton droit sur l’application d’invite de commandes, puis sélectionnez Exécuter en **tant qu’administrateur.** Si vous êtes invité à obtenir un mot de passe d’administrateur ou une confirmation, tapez le mot de passe ou cliquez sur **Autoriser.**  

2. Dans la fenêtre Invite de commandes, tapez **dsregcmd /leave**  et attendez que la commande se termine. Tapez **ensuite dsregcmd /join** et attendez la fin de la commande.
3. Redémarrez votre ordinateur.
