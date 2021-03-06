---
title: Bloquer les signatures électroniques de l’utilisateur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464619"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="4b2dc-102">Bloquer les signatures électroniques de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="4b2dc-102">Block user-made email signatures</span></span>

<span data-ttu-id="4b2dc-103">La solution suivante s’applique uniquement aux signatures électroniques créées dans Outlook sur le web.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="4b2dc-104">Vous ne pouvez bloquer les signatures dans l’application Outlook que si vous avez une Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="4b2dc-105">Dans le Centre d’administration, sélectionnez **Centres d’administration**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="4b2dc-106">Cliquez sur **autorisations**  >  **Stratégies Outlook Web App.**</span><span class="sxs-lookup"><span data-stu-id="4b2dc-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="4b2dc-107">Sélectionnez la stratégie, puis cliquez sur l’icône de crayon pour la modifier.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="4b2dc-108">Cliquez sur  >  **fonctionnalités Plus d’options**.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="4b2dc-109">Sous **Expérience utilisateur,** cochez la case **Signature** électronique, puis cliquez sur **Enregistrer.**</span><span class="sxs-lookup"><span data-stu-id="4b2dc-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="4b2dc-110">**Important :** Si une signature a été ajoutée avant d’effacer cette case à cocher, l’utilisateur pourra toujours l’utiliser.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="4b2dc-111">Demandez-leur de le supprimer.</span><span class="sxs-lookup"><span data-stu-id="4b2dc-111">Ask them to remove it.</span></span>