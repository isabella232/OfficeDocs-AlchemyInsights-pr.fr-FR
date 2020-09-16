---
title: 'Le client Teams se bloque :'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691105"
---
# <a name="teams-client-crashing"></a>Le client Teams se bloque :

Si votre client Teams se bloque, procédez comme suit :

- Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Assurez-vous que toutes les [plages d’adresses et d’URL Microsoft 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) sont accessibles.

- Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.

- Désinstaller et réinstaller l’application Teams (lien)
    - Accédez au dossier %appdata%\Microsoft\teams\ sur votre ordinateur et supprimez tous les fichiers dans ce répertoire.
    - [Téléchargez et installez l’application Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)et, si possible, installez teams en tant qu’administrateur (cliquez avec le bouton droit sur le programme d’installation Teams, puis sélectionnez « Exécuter en tant qu’administrateur » si disponible).

Si votre client Teams ne fonctionne toujours pas, pouvez-vous reproduire le problème ? Si c’est le cas :

1. Utilisez l’Enregistreur d’actions pour capturer vos étapes.
    - Fermez TOUTES les applications superflues ou confidentielles.
    - Lancez l’Enregistreur d’actions et reproduisez le problème lors de la connexion avec le compte d’utilisateur concerné.
    - [Collecter les journaux des équipes qui capturent les étapes de reproduction enregistrées](https://docs.microsoft.com/microsoftteams/log-files). **Remarque** : Veillez à capturer l’adresse de connexion de l’utilisateur concerné.
    - Collectez les informations de copie de sauvegarde et/ou de compartiment défectueux (Windows). Lancez Windows PowerShell sur l’ordinateur sur lequel le blocage se produit et exécutez les commandes suivantes :

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Joignez le fichier à votre cas de support.
