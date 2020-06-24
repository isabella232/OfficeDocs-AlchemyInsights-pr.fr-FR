---
title: Autorisations de calendrier
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44854010"
---
# <a name="calendar-permissions"></a>Autorisations de calendrier

Les utilisateurs peuvent modifier leurs propres autorisations de calendrier avec Outlook sur le Web ou d’autres clients, mais en tant qu’administrateur, vous devrez peut-être également enquêter.  
Avec l’applet de commande Exchange PowerShell affiche l’autorisation sur le calendrier d’un utilisateur :

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Pour plus d’informations, consultez les rubriques suivantes :

- [Get-MailboxFolderPermission permet](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission permet](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission permet](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Les autorisations de calendrier sont utilisées dans le partage des calendriers, pour plus d’informations sur le partage d’un calendrier Outlook, consultez les articles suivants :

- [Partager un calendrier Outlook avec d’autres personnes](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Partager votre calendrier dans Outlook sur le Web pour les entreprises](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Pour résoudre les problèmes liés à l’autorisation de calendrier, vous pouvez utiliser l’outil [support et Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .