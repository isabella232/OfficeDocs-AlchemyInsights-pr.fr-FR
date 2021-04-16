---
title: 0x8004de40'erreur lors du lancement de OneDrive
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
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813650"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40'erreur lors du lancement de OneDrive

Si vous recevez un message **d'0x8004de40** lors de la connexion à OneDrive, redémarrez l'ordinateur lorsque vous êtes connecté à votre domaine scolaire ou scolaire. Si vous recevez cette erreur après le redémarrage, essayez ceci lorsque vous êtes connecté à votre domaine scolaire ou scolaire :

1. Cliquez sur Démarrer, puis tapez **cmd** **ou** invite de commandes dans la zone de recherche, cliquez avec le bouton droit sur l'application d'invite de commandes, puis sélectionnez Exécuter en **tant qu'administrateur.** Si vous êtes invité à obtenir un mot de passe d'administrateur ou une confirmation, tapez le mot de passe ou cliquez sur **Autoriser.**  

2. Dans la fenêtre Invite de commandes, tapez **dsregcmd /leave**  et attendez que la commande se termine. Tapez **ensuite dsregcmd /join** et attendez la fin de la commande.
3. Redémarrez votre ordinateur.
