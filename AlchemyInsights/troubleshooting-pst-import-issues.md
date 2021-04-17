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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826161"
---
# <a name="troubleshooting-pst-import-issues"></a>Résolution de problèmes d’importation PST

- Si vous effectuez l’importation dans le client Outlook lui-même, consultez [Résoudre les problèmes d’importation d’un fichier .pst Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Si vous utilisez le service d’importation et que celui-ci est bloqué, veuillez noter que la taille de chaque fichier PST téléchargé vers l’emplacement de stockage Azure ne doit pas dépasser 20 Go. Les fichiers PST d’une taille supérieure à 20 Go peuvent avoir un impact sur les performances du processus d’importation PST.

- Si vous voulez vérifier l’état d’une tâche spécifique d’importation, vous pouvez utiliser [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Pour plus d’informations sur le service d’importation, consultez la [Vue d’ensemble de l’importation des fichiers PST de votre organisation](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
