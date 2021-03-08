---
title: Déplacer automatiquement les messages électroniques vers la boîte aux lettres d’archivage
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522390"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="470f3-102">Déplacer automatiquement les messages électroniques vers la boîte aux lettres d’archivage</span><span class="sxs-lookup"><span data-stu-id="470f3-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="470f3-103">Voici comment configurer une stratégie pour déplacer automatiquement l’ancien courrier électronique d’un utilisateur vers la boîte aux lettres d’archivage :</span><span class="sxs-lookup"><span data-stu-id="470f3-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="470f3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143)Data  >  **governance**  >  **Archive** to verify an archive mailbox has been enabled for the user.</span><span class="sxs-lookup"><span data-stu-id="470f3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="470f3-105">Si ce n’est pas le cas, cliquez sur **Activer,** **puis Oui** dans la zone d’avertissement.</span><span class="sxs-lookup"><span data-stu-id="470f3-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="470f3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="470f3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="470f3-107">Choisissez l’icône + puis **sélectionnez appliquer automatiquement à la boîte aux lettres entière.**</span><span class="sxs-lookup"><span data-stu-id="470f3-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="470f3-108">Attribuez un nom à la balise de rétention, puis choisissez **Déplacer vers l’archive.**</span><span class="sxs-lookup"><span data-stu-id="470f3-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="470f3-109">Pour la période de rétention, entrez l’heure que vous souhaitez, par exemple 90 jours.</span><span class="sxs-lookup"><span data-stu-id="470f3-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="470f3-110">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="470f3-110">Click **Save**.</span></span>
5. <span data-ttu-id="470f3-111">Maintenant, créez une stratégie de rétention : choisissez des **stratégies de** rétention, choisissez l’icône pour ajouter une nouvelle stratégie.</span><span class="sxs-lookup"><span data-stu-id="470f3-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="470f3-112">Attribuez un nom à la stratégie de rétention, puis cliquez et faites défiler pour rechercher et ajouter la balise de rétention que vous vient de créer.</span><span class="sxs-lookup"><span data-stu-id="470f3-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="470f3-113">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="470f3-113">Click **Save**.</span></span>
7. <span data-ttu-id="470f3-114">Enfin, appliquez la stratégie de rétention à la boîte aux lettres de l’utilisateur : toujours dans le Centre d’administration Exchange, allez aux boîtes aux **lettres des**  >  **destinataires.**</span><span class="sxs-lookup"><span data-stu-id="470f3-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="470f3-115">Choisissez tous les utilisateurs à qui vous souhaitez appliquer la stratégie, puis sélectionnez **Modifier** (icône de crayon).</span><span class="sxs-lookup"><span data-stu-id="470f3-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="470f3-116">Dans la boîte de dialogue, cliquez sur **fonctionnalités de boîte aux lettres.**</span><span class="sxs-lookup"><span data-stu-id="470f3-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="470f3-117">Sous **Stratégie de rétention,** appliquez la stratégie que vous avez créée > **Enregistrer.**</span><span class="sxs-lookup"><span data-stu-id="470f3-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="470f3-118">Pour obtenir des instructions sur l’application de la stratégie à tous les utilisateurs, voir [Appliquer une stratégie de rétention aux boîtes aux lettres.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="470f3-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
