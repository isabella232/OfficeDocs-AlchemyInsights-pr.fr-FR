---
title: 'Le client Teams se bloque :'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030585"
---
# <a name="teams-client-crashing"></a>Le client Teams se bloque :

Si votre client Teams se bloque, procédez comme suit :

- Si vous utilisez l’application de bureau Teams, [vérifiez que l’application est totalement mise à jour](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Veillez à ce que toutes les [plages d’adresses et d’URL Office 365 ](https://docs.microsoft.com/microsoftteams/connectivity-issues) sont accessibles.

- Connectez-vous à l’aide de votre compte d’administrateur et consultez votre [Tableau de bord d’état du service](https://docs.microsoft.com/office365/enterprise/view-service-health) pour vérifier qu’il n’existe aucune panne ou détérioration du service.

 - Pour terminer, vous pouvez essayer de vider le cache de votre client Teams :

    1.  Quittez complètement le client de bureau Microsoft Teams. Vous pouvez cliquer avec le bouton droit sur **Teams** à partir de Icon Tray, puis cliquez sur **Quitter** ou exécutez le Gestionnaire des tâches et terminez complètement le processus.

    2.  Accédez à l’Explorateur de fichiers, puis tapez %appdata%\Microsoft\teams.

    3.  Une fois que vous êtes dans l’annuaire, quelques-uns des dossiers suivants s’affichent :

         - Dans **Application Cache**, accédez à Cache et supprimez les fichiers dans l’emplacement du Cache : %appdata%\Microsoft\teams\application cache\cache.

        - Dans **Blob_storage**, supprimez tous les fichiers : %appdata%\Microsoft\teams\blob_storage.

        - Dans **Cache**, supprimez tous les fichiers : %appdata%\Microsoft\teams\Cache.

        - Dans **databases**, supprimez tous les fichiers : %appdata%\Microsoft\teams\databases.

        - Dans **GPUCache**, supprimez tous les fichiers : %appdata%\Microsoft\teams\GPUcache.

        - Dans **IndexedDB**, supprimez le fichier .db : %appdata%\Microsoft\teams\IndexedDB.

        - Dans **Local Stockage**, supprimez tous les fichiers : %appdata%\Microsoft\teams\Local Storage.

        - Enfin, dans **tmp**, supprimez les fichiers suivants : %appdata%\Microsoft\teams\tmp.

    4. Redémarrez le client Teams.
