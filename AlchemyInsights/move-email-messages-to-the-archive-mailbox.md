---
title: Déplacer des messages électroniques vers la boîte aux lettres d’archivage
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379495"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="a6e9a-102">Déplacer le courrier électronique vers la boîte aux lettres d’archivage</span><span class="sxs-lookup"><span data-stu-id="a6e9a-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="a6e9a-103">Vérifiez qu’une **boîte aux lettres** d’archivage a été activée.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="a6e9a-104">Si ce n’est pas le cas, suivez les étapes décrites dans [cet article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) pour activer la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="a6e9a-105">Pour archiver automatiquement les messages dans la boîte aux lettres d’archivage, une balise de rétention avec l’action **déplacer vers l’archive** doit être définie sur **appliqué automatiquement à la balise de boîte aux lettres (par défaut) entière**.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="a6e9a-106">Suivez les étapes ci-dessous pour créer la balise: [archive default](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="a6e9a-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>

3. <span data-ttu-id="a6e9a-107">Ensuite, ajoutez la balise **Archive** à votre stratégie de rétention.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="a6e9a-108">Dans le centre d’administration Exchange, choisissez **stratégies** de rétention > ajouter la **balise déplacer vers l’archive** à la stratégie > **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="a6e9a-109">À présent, [affectez la stratégie](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) de rétention à la boîte aux lettres de l’utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="a6e9a-110">La même stratégie sera appliquée à la boîte aux lettres **principale** et à la boîte aux lettres d' **archivage** .</span><span class="sxs-lookup"><span data-stu-id="a6e9a-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="a6e9a-111">Il peut s’avérer nécessaire de forcer l’Assistant dossier géré à exécuter et d’appliquer les nouveaux paramètres à la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a6e9a-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="a6e9a-112">Exécutez la commande suivante lorsque [vous êtes connecté à exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique:</span><span class="sxs-lookup"><span data-stu-id="a6e9a-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="a6e9a-113">Start-ManagedFolderAssistant-Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="a6e9a-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="a6e9a-114">Pour plus d’informations sur la configuration d’une stratégie d’archivage, consultez la rubrique [configurer une stratégie d’archivage et de suppression pour les boîtes aux lettres](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="a6e9a-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  