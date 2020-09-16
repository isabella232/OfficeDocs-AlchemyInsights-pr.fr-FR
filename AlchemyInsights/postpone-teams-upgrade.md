---
title: Différer la mise à niveau des équipes
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741769"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Ajournement de la mise à niveau des équipes basées sur Microsoft

**Important**: nous pouvons vous aider à résoudre ce problème pour vous en utilisant un diagnostic du support technique, mais il semble que vous n’utilisiez pas le nouveau centre d’administration. Pour utiliser le nouveau centre d’administration, faites glisser le bouton bascule en haut à droite qui indique **nouveau centre d’administration** à droite. À l’aide du nouveau centre d’administration, cliquez sur le widget **besoin d’aide ?** , tapez « différer la mise à niveau des équipes », puis suivez les invites pour exécuter le diagnostic.

Si vous avez reçu une communication sur une mise à niveau automatisée basée sur Microsoft de Skype entreprise vers Microsoft teams et que vous souhaitez reporter la mise à niveau automatique à une date ultérieure, votre administrateur général peut se connecter au [portail d’administration de teams](https://admin.teams.microsoft.com/dashboard) et, après avoir sélectionné le bouton **Actualiser** dans la section mise à niveau de Microsoft Teams, sélectionnez le bouton **reporter** . Pour afficher la nouvelle date de mise à niveau automatisée de votre client vers Microsoft Teams, actualisez la page du portail d’administration de teams.

**Remarque :** Le bouton **reporter** n’est disponible que si vous avez reçu la notification du centre de messages concernant la mise à niveau automatisée. 

Les administrateurs globaux peuvent également exécuter [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) pour en savoir plus sur l’état actuel de la mise à niveau.
