---
title: Résolution de problèmes d’importation PST
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
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972417"
---
# <a name="troubleshooting-pst-import-issues"></a>Résolution de problèmes d’importation PST

- Si vous effectuez l’importation dans le client Outlook lui-même, consultez [Résoudre les problèmes d’importation d’un fichier .pst Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Si vous utilisez le service d’importation et que celui-ci est bloqué, veuillez noter que la taille de chaque fichier PST chargé vers l’emplacement de stockage Azure ne doit pas dépasser 20 Go. Les fichiers PST d’une taille supérieure à 20 Go peuvent avoir un impact sur les performances du processus d’importation PST. Pour plus d’informations sur la résolution des problèmes de tâches bloquées, consultez les [problèmes qui affectent les tâches d’importation PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Si vous voulez vérifier l’état d’une tâche spécifique d’importation, vous pouvez utiliser [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Pour plus d’informations sur le service d’importation, consultez la [Vue d’ensemble de l’importation des fichiers PST de votre organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
