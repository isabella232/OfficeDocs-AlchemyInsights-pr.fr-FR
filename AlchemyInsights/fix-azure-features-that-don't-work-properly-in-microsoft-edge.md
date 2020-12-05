---
title: Procédure à suivre si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576408"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="b5488-102">Procédure à suivre si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="b5488-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="b5488-103">Microsoft Edge présente des [problèmes connus](https://go.microsoft.com/fwlink/?linkid=2140608) liés aux zones de sécurité et peut influer sur la façon dont les utilisateurs Azure se connectent au centre d’administration Windows.</span><span class="sxs-lookup"><span data-stu-id="b5488-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="b5488-104">Si vous rencontrez des problèmes lors de l’utilisation des fonctionnalités Azure avec Microsoft Edge, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="b5488-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="b5488-105">Dans le menu **Démarrer** , recherchez **Options Internet** et sélectionnez-le.</span><span class="sxs-lookup"><span data-stu-id="b5488-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="b5488-106">Dans la boîte de dialogue **Propriétés Internet** , accédez à l’onglet **sécurité** .</span><span class="sxs-lookup"><span data-stu-id="b5488-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="b5488-107">Sélectionnez la zone **sites de confiance** , puis cliquez sur le bouton **sites** .</span><span class="sxs-lookup"><span data-stu-id="b5488-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="b5488-108">Dans la boîte de dialogue **sites de confiance** , ajoutez votre URL de passerelle, ainsi que [https://login.microsoftonline.com](https://login.microsoftonline.com) et, puis [https://login.live.com](https://login.live.com) sélectionnez **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="b5488-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="b5488-109">Dans la boîte de dialogue **Propriétés Internet** , accédez à l’onglet **confidentialité** .</span><span class="sxs-lookup"><span data-stu-id="b5488-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="b5488-110">Dans la section **bloqueur de fenêtres publicitaires intempestives** , sélectionnez **paramètres**.</span><span class="sxs-lookup"><span data-stu-id="b5488-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="b5488-111">Dans la boîte de dialogue qui s’ouvre, ajoutez votre URL de passerelle, ainsi que [https://login.microsoftonline.com](https://login.microsoftonline.com) et [https://login.live.com](https://login.live.com) , puis sélectionnez **Fermer**.</span><span class="sxs-lookup"><span data-stu-id="b5488-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
