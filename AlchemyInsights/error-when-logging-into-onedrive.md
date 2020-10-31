---
title: erreur 0x8004de40 lors du lancement de OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815991"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>erreur 0x8004de40 lors du lancement de OneDrive

Si vous recevez un message d’erreur **0x8004de40** lors de la connexion à OneDrive, redémarrez l’ordinateur tout en étant connecté à votre domaine professionnel ou scolaire. Si vous recevez cette erreur après avoir redémarré, essayez ceci en vous connectant à votre domaine professionnel ou scolaire :

1. Cliquez sur Démarrer, puis tapez **cmd** ou **invite de commandes**  dans la zone de recherche, cliquez avec le bouton droit sur l’application invite de commandes, puis sélectionnez  **exécuter en tant qu’administrateur** . Si vous êtes invité à entrer un mot de passe d’administrateur ou une confirmation, tapez le mot de passe, ou cliquez sur **autoriser** .  

2. Dans la fenêtre d’invite de commandes, tapez **dsregcmd/Leave**  et attendez la fin de la commande. Tapez ensuite **dsregcmd/Join** et attendez la fin de la commande.
3. Redémarrez votre ordinateur.
