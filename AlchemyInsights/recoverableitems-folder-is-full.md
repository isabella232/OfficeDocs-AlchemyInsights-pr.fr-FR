---
title: 1336 le dossier RecoverableItems est plein
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510750"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="dd025-102">Le dossier éléments récupérables est plein</span><span class="sxs-lookup"><span data-stu-id="dd025-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="dd025-103">Pour les boîtes aux lettres Exchange Online, la limite de stockage par défaut pour le dossier éléments récupérables est de 30 Go.</span><span class="sxs-lookup"><span data-stu-id="dd025-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="dd025-104">La limite de stockage pour le dossier éléments récupérables est automatiquement augmentée à 100 Go si la boîte aux lettres est placée en conservation pour litige, conservation eDiscovery ou si elle est affectée à une stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="dd025-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="dd025-105">Lorsque le dossier éléments récupérables atteint la limite de stockage, la fonctionnalité de boîte aux lettres est affectée des manières suivantes :</span><span class="sxs-lookup"><span data-stu-id="dd025-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="dd025-106">L’utilisateur ne peut pas supprimer des éléments de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dd025-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="dd025-107">L'Assistant Dossier géré ne peut pas supprimer des éléments en fonction de la balise de rétention ou des paramètres de dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="dd025-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="dd025-108">Pour les boîtes aux lettres pour lesquelles la récupération d’élément unique est activée ou qui sont placées en conservation, le processus de protection de page de copie sur écriture ne peut pas conserver les versions des éléments modifiés par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="dd025-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="dd025-109">Pour les boîtes aux lettres pour lesquelles l’enregistrement d’audit de boîte aux lettres est activé, aucune entrée de journal d’audit de boîte aux lettres ne peut être enregistrée dans le sous-dossier audits du dossier éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="dd025-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="dd025-110">Pour les boîtes aux lettres qui ne sont pas en attente, les administrateurs peuvent utiliser la `Search-Mailbox -SearchDumpsterOnly -DeleteContent` commande dans Exchange Online PowerShell pour supprimer des éléments dans le dossier éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="dd025-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="dd025-111">Pour plus d’informations, voir les rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="dd025-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="dd025-112">Rechercher et supprimer des messages</span><span class="sxs-lookup"><span data-stu-id="dd025-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="dd025-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="dd025-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="dd025-114">Pour les boîtes aux lettres en attente, les administrateurs doivent supprimer le blocage avant de pouvoir supprimer des éléments du dossier éléments récupérables.</span><span class="sxs-lookup"><span data-stu-id="dd025-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="dd025-115">Pour plus d’informations, consultez [la rubrique supprimer des éléments dans le dossier éléments récupérables des boîtes aux lettres en nuage en conservation](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="dd025-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="dd025-116">Pour éviter que le dossier éléments récupérables ne devienne saturé, les administrateurs peuvent augmenter la limite de stockage du dossier éléments récupérables pour les boîtes aux lettres en attente et configurer une stratégie de rétention de boîte aux lettres qui déplace les éléments du dossier éléments récupérables vers la boîte aux lettres d’archivage de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="dd025-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="dd025-117">Voir [augmenter le quota des éléments récupérables pour les boîtes aux lettres en attente](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="dd025-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
