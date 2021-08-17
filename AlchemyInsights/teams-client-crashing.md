---
title: Blocage du client Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890336"
---
# <a name="teams-client-crashing"></a>Blocage du client Teams

Si votre client Teams se bloque, procédez comme suit :

- Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assurez-vous que toutes les [plages d’adresses et d’URL Microsoft 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) sont accessibles.

- Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.

- Désinstaller et réinstaller l’application Teams
    - Accédez au dossier %appdata%\Microsoft\Teams\ sur votre ordinateur et supprimez tous les fichiers dans ce répertoire.
    - [Téléchargez et installez l’application Teams](https://www.microsoft.com/microsoft-teams/download-app)et, si possible, installez teams en tant qu’administrateur (cliquez avec le bouton droit sur le programme d’installation Teams, puis sélectionnez **Exécuter en tant qu’administrateur** si disponible).

Si votre client Teams se bloque toujours, essayez de reproduire le problème. Si vous pouvez :

1. Utilisez l’Enregistreur d’actions pour capturer vos étapes.
    - Fermez TOUTES les applications superflues ou confidentielles.
    - Lancez l’Enregistreur d’actions et reproduisez le problème lors de la connexion avec le compte d’utilisateur concerné.
    - [Collecter les journaux des équipes qui capturent les étapes de reproduction enregistrées](https://docs.microsoft.com/microsoftteams/log-files). **Remarque** : Veillez à capturer l’adresse de connexion de l’utilisateur concerné.
    - Collectez les informations de vidage et/ou de compartiment d’erreur (Windows). Lancez Windows Powershell sur l’ordinateur sur lequel le blocage se produit et exécutez les commandes suivantes (après chaque commande, appuyez sur Entrée) :

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Une fois le fichier texte généré et affiché à l’écran, enregistrez le fichier et attachez-le à la demande de service. 
