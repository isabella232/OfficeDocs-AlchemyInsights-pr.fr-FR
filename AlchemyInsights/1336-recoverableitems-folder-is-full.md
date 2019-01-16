---
title: Le dossier RecoverableItems 1336 est plein
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: ee96abfa179c36ebaf43dbd327d4608b849395d3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288111"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="e48ab-102">Le dossier éléments récupérables est plein</span><span class="sxs-lookup"><span data-stu-id="e48ab-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="e48ab-p101">Pour les boîtes aux lettres Exchange Online dans Office 365, la limite de stockage par défaut pour le dossier éléments récupérables est de 30 Go. La limite de stockage pour le dossier éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placé en blocage pour litige, blocage eDiscovery, ou est affecté à une stratégie de rétention d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="e48ab-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="e48ab-105">Lorsque le dossier éléments récupérables atteint la limite de stockage, les fonctionnalités de boîte aux lettres sont affectée de la manière suivante :</span><span class="sxs-lookup"><span data-stu-id="e48ab-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="e48ab-106">L’utilisateur ne peut pas supprimer des éléments dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e48ab-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="e48ab-107">L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="e48ab-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="e48ab-108">Pour les boîtes aux lettres de récupération d’élément unique ou sont mis en attente, le processus de protection de page de la copie sur écriture ne peut pas mettre à jour les versions des éléments modifiés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e48ab-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="e48ab-109">Pour les boîtes aux lettres dont les boîtes aux lettres d’audit de l’enregistrement est activé, aucune entrée du journal d’audit boîte aux lettres ne peut être enregistrées dans le sous-dossier des Audits dans le dossier éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="e48ab-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="e48ab-p102">Pour les boîtes aux lettres qui ne sont pas en attente, les administrateurs peuvent utiliser le `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command dans Exchange Online PowerShell pour supprimer des éléments dans le dossier éléments récupérables. Pour plus d’informations, voir les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="e48ab-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="e48ab-112">Rechercher et supprimer des messages</span><span class="sxs-lookup"><span data-stu-id="e48ab-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="e48ab-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="e48ab-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="e48ab-p103">Pour les boîtes aux lettres qui sont en attente, administrateurs doivent retirer le blocage avant de pouvoir les éléments supprimés du dossier éléments récupérables. Pour plus d’informations, voir [Supprimer des éléments dans les éléments récupérables dossier de boîtes aux lettres en nuage sur contenir](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="e48ab-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/en-us/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="e48ab-p104">Pour vous aider à empêcher la saturation du dossier éléments récupérables, administrateurs peuvent augmenter la limite de stockage des éléments récupérables dossier pour les boîtes aux lettres sur Maintenez et définir une stratégie de rétention de boîte aux lettres qui déplace les éléments à partir du dossier éléments récupérables pour l’archivage de l’utilisateur boîte aux lettres. Voir [augmenter les éléments récupérables quota de boîtes aux lettres sur Maintenez](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="e48ab-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

