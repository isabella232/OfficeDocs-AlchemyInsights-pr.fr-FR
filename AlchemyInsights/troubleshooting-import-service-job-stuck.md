---
title: Dépannage du blocage de la tâche du service d’importation
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059844"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Dépannage du blocage de la tâche du service d’importation

Si vous rencontrez des problèmes avec des tâches de service d’importation bloquées ou défaillantes, examinez et essayez ceci :

- Examinez la taille du fichier PST. La taille maximale recommandée d’un fichier PST pour l’importation est de 20 Go.

- Si vous pensez que des éléments ont été ignorés en raison d’une corruption, exécutez Scanpst.exe pour diagnostiquer et corriger les erreurs dans les fichiers PST.

- Si vous voyez une erreur « MapiExceptionShutoffÉléceed » lors de l’importation, assurez-vous que la boîte aux lettres cible dispose des capacités suffisantes pour importer les fichiers PST souhaités.

Pour plus d’informations sur la résolution des problèmes liés à la tâche d’importation de données PST, consultez [Résoudre les problèmes liés aux tâches d’importation PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

Pour plus d’informations sur la correction des problèmes lors de l’importation de fichiers PST dans Outlook, consultez [Résoudre les problèmes d’importation d’un fichier .pst Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).