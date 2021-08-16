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
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100216"
---
# <a name="teams-doesnt-launch"></a>Teams ne se lance pas

Si vous tentez d’ouvrir Microsoft Teams et qu’il ne se lance pas, essayez ce qui suit :

1. Accédez à **%AppData%\Microsoft\Teams**.
1. Supprimer le contenu du dossier.
1. Redémarrez l’ordinateur, puis essayez de lancer Teams.

Vous devez peut-être réinstaller Teams. Pour réinstaller :

1. Désinstallez Teams à l’aide du Panneau de configuration.
1. Accédez à **%AppData%\Microsoft\Teams\Applications Cache**.
1. Supprimer le contenu du dossier.
1. Accédez à **%AppData%\Microsoft\teams\Cache**.
1. Supprimer le contenu du dossier.
1. Redémarrez l’ordinateur, puis téléchargez et installez Teams.

Si vous souhaitez exécuter un diagnostic sur votre client pour un utilisateur spécifique qui ne peut pas se connecter, démarrez une nouvelle rechercher avec le mot clé **TeamsUserUnableToSignIn**, puis suivez les invites.