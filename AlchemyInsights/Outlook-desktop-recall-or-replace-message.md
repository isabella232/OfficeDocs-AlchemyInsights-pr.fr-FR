---
title: Rappel du Bureau Outlook ou remplacement d’un message électronique
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663988"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="263d6-102">Rappeler ou remplacer un message électronique Outlook</span><span class="sxs-lookup"><span data-stu-id="263d6-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="263d6-103">En tant qu’administrateur, vous pouvez **rappeler des messages au nom des utilisateurs à l’aide de PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="263d6-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="263d6-104">Vous ne pouvez pas rappeler les messages à partir du centre d’administration.</span><span class="sxs-lookup"><span data-stu-id="263d6-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="263d6-105">Vous pouvez **uniquement rappeler les messages qui sont envoyés à des personnes de votre organisation**.</span><span class="sxs-lookup"><span data-stu-id="263d6-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="263d6-106">Si le message a été envoyé à une adresse Gmail, par exemple, vous ne pouvez pas le rappeler.</span><span class="sxs-lookup"><span data-stu-id="263d6-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="263d6-107">Vous pouvez **uniquement rappeler les messages envoyés à partir d’Outlook 2016 sur le PC**.</span><span class="sxs-lookup"><span data-stu-id="263d6-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="263d6-108">Si un utilisateur envoie un message à l’aide d’Outlook pour Mac ou d’Outlook sur le Web, vous ne pouvez pas le rappeler.</span><span class="sxs-lookup"><span data-stu-id="263d6-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="263d6-109">Pour rappeler ou remplacer un message électronique :</span><span class="sxs-lookup"><span data-stu-id="263d6-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="263d6-110">Dans le volet des dossiers situé à gauche de la fenêtre Outlook, sélectionnez le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="263d6-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="263d6-111">Double-cliquez sur le message que vous souhaitez rappeler pour l’ouvrir.</span><span class="sxs-lookup"><span data-stu-id="263d6-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="263d6-112">Sélectionnez l’onglet **message** , puis sélectionnez **actions**  >  **rappeler ce message**.</span><span class="sxs-lookup"><span data-stu-id="263d6-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="263d6-113">Sélectionnez **Supprimer les copies non lues de ce message** ou **Supprimer les copies non lues et les remplacer par un nouveau message**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="263d6-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="263d6-114">Si vous envoyez un message de remplacement, composez le message, puis sélectionnez **Envoyer**.</span><span class="sxs-lookup"><span data-stu-id="263d6-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="263d6-115">La réussite ou l’échec d’un rappel de message dépend des paramètres du destinataire dans Outlook.</span><span class="sxs-lookup"><span data-stu-id="263d6-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="263d6-116">Pour connaître les étapes à suivre pour vérifier le rappel, consultez [cet article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="263d6-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="263d6-117">Recherche et suppression de messages électroniques dans votre organisation</span><span class="sxs-lookup"><span data-stu-id="263d6-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="263d6-118">Si vous n’êtes pas un administrateur général, votre compte doit être ajouté au rôle gestionnaire eDiscovery ou au rôle de gestion de la recherche de conformité pour rechercher des messages.</span><span class="sxs-lookup"><span data-stu-id="263d6-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="263d6-119">Pour supprimer des messages, vous devez rejoindre le groupe de rôles gestion de l’organisation ou le rôle de gestion de la recherche et de la purge.</span><span class="sxs-lookup"><span data-stu-id="263d6-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="263d6-120">Les autorisations de ces rôles sont attribuées dans le [Centre de sécurité et de conformité](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="263d6-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="263d6-121">[Créer une recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/content-search) pour rechercher le message à supprimer.</span><span class="sxs-lookup"><span data-stu-id="263d6-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="263d6-122">[Connectez-vous au centre de sécurité et de conformité PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="263d6-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="263d6-123">Si vous utilisez l’authentification multifacteur, reportez-vous [à se connecter au centre de sécurité et de conformité Microsoft 365 PowerShell à l’aide de l’authentification multifacteur](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="263d6-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>