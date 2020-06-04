---
title: Messages manquants en quarantaine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542152"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="219ec-102">Messages manquants en quarantaine</span><span class="sxs-lookup"><span data-stu-id="219ec-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="219ec-103">Les administrateurs peuvent [afficher, publier ou supprimer ces messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="219ec-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="219ec-104">Pour ouvrir le centre de sécurité & conformité, accédez à [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="219ec-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="219ec-105">Pour ouvrir la page de mise en quarantaine directement, accédez à [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="219ec-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="219ec-106">Vous pouvez effectuer une recherche sur les valeurs suivantes :</span><span class="sxs-lookup"><span data-stu-id="219ec-106">You can search by the following values:</span></span>  

- <span data-ttu-id="219ec-107">**ID du message** : l’identificateur global unique du message.</span><span class="sxs-lookup"><span data-stu-id="219ec-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="219ec-108">Si vous sélectionnez un message dans la liste, la valeur de l' **ID du message** s’affiche dans le volet flyout de **Détails** qui s’affiche.</span><span class="sxs-lookup"><span data-stu-id="219ec-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="219ec-109">Les administrateurs peuvent utiliser le [suivi des messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) pour rechercher les messages et les valeurs d’ID de message correspondantes.</span><span class="sxs-lookup"><span data-stu-id="219ec-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="219ec-110">**Adresse e-mail de l'expéditeur** : adresse e-mail d'un seul expéditeur.</span><span class="sxs-lookup"><span data-stu-id="219ec-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="219ec-111">**Adresse e-mail du destinataire** : adresse e-mail d'un seul destinataire.</span><span class="sxs-lookup"><span data-stu-id="219ec-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="219ec-112">**Sujet** : utiliser l'intégralité du sujet du message.</span><span class="sxs-lookup"><span data-stu-id="219ec-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="219ec-113">La recherche n’est pas sensible à la casse.</span><span class="sxs-lookup"><span data-stu-id="219ec-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="219ec-114">Une fois que vous avez entré les critères de recherche, cliquez sur Actualiser ![ le bouton ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Actualiser** pour filtrer les résultats.  </span><span class="sxs-lookup"><span data-stu-id="219ec-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="219ec-115">Les cmdlets que vous utilisez pour afficher et gérer les messages et les fichiers en quarantaine sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="219ec-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="219ec-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="219ec-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="219ec-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="219ec-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="219ec-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="219ec-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="219ec-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Notez que cette applet de commande concerne uniquement les messages, pas les fichiers de programmes malveillants, pour SharePoint Online, OneDrive entreprise ou Teams.</span><span class="sxs-lookup"><span data-stu-id="219ec-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="219ec-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="219ec-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)