---
title: Autorisations de calendrier
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
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748791"
---
# <a name="calendar-permissions"></a><span data-ttu-id="0ed97-102">Autorisations de calendrier</span><span class="sxs-lookup"><span data-stu-id="0ed97-102">Calendar Permissions</span></span>

<span data-ttu-id="0ed97-103">Les utilisateurs peuvent modifier leurs propres autorisations de calendrier avec Outlook sur le Web ou d’autres clients, mais en tant qu’administrateur, vous devrez peut-être également enquêter.</span><span class="sxs-lookup"><span data-stu-id="0ed97-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="0ed97-104">Avec l’applet de commande Exchange PowerShell affiche l’autorisation sur le calendrier d’un utilisateur :</span><span class="sxs-lookup"><span data-stu-id="0ed97-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="0ed97-105">Pour plus d’informations, consultez les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="0ed97-105">To see more information see the following:</span></span>

- [<span data-ttu-id="0ed97-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="0ed97-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="0ed97-107">Set-MailboxFolderPermission permet</span><span class="sxs-lookup"><span data-stu-id="0ed97-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="0ed97-108">Add-MailboxFolderPermission permet</span><span class="sxs-lookup"><span data-stu-id="0ed97-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="0ed97-109">Les autorisations de calendrier sont utilisées dans le partage des calendriers, pour plus d’informations sur le partage d’un calendrier Outlook, consultez les articles suivants :</span><span class="sxs-lookup"><span data-stu-id="0ed97-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="0ed97-110">Partager un calendrier Outlook avec d’autres personnes</span><span class="sxs-lookup"><span data-stu-id="0ed97-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="0ed97-111">Partager votre calendrier dans Outlook sur le Web pour les entreprises</span><span class="sxs-lookup"><span data-stu-id="0ed97-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="0ed97-112">Pour résoudre les problèmes liés à l’autorisation de calendrier, vous pouvez utiliser l’outil [support et Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="0ed97-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>