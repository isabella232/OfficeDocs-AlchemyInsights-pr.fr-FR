---
title: Teams ne se lance pas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329324"
---
# <a name="teams-doesnt-launch"></a>Teams ne se lance pas

Si vous tentez d’ouvrir Microsoft Teams et qu’il ne se lance pas, essayez ce qui suit :

1. Accédez à **%AppData%\Microsoft\Teams**.
1. Supprimer le contenu du dossier.
1. Redémarrez l’ordinateur, puis essayez de lancer Teams.

Vous devrez peut-être réinstaller Teams. Pour réinstaller:

1. Désinstallez Teams à l’aide du Panneau de configuration.
1. Accédez à **%AppData%\Microsoft\Teams\Applications Cache**.
1. Supprimer le contenu du dossier.
1. Accédez à **%AppData%\Microsoft\teams\Cache**.
1. Supprimer le contenu du dossier.
1. Redémarrez l’ordinateur, puis téléchargez et installez Teams.

Si vous souhaitez exécuter un diagnostic sur votre client pour un utilisateur spécifique qui ne peut pas se connecter, démarrez une nouvelle rechercher avec le mot clé **TeamsUserUnableToSignIn**, puis suivez les invites.