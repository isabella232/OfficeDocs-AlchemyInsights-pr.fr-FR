---
title: Corriger la stratégie de client (remplacement d’action)
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
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736684"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="6bfce-102">Corriger la stratégie de client (remplacement d’action)</span><span class="sxs-lookup"><span data-stu-id="6bfce-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="6bfce-103">Une stratégie anti-courrier indésirable dans votre client a affecté ce message.</span><span class="sxs-lookup"><span data-stu-id="6bfce-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="6bfce-104">Pour passer en revue la stratégie, faites les choses suivantes :</span><span class="sxs-lookup"><span data-stu-id="6bfce-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="6bfce-105">Go to the [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)and then go to **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="6bfce-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="6bfce-106">Vérifiez si la **source de** stratégie indique les éléments suivants :  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="6bfce-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="6bfce-107">Si c’est le cas, sous **l’onglet** Personnalisé, vérifiez les paramètres de la stratégie qui a affecté le message.</span><span class="sxs-lookup"><span data-stu-id="6bfce-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="6bfce-108">Il est possible que les **paramètres Standard appliqués** à tous les clients Exchange Online Protection affectent le message.</span><span class="sxs-lookup"><span data-stu-id="6bfce-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="6bfce-109">Pour plus d’informations sur la configuration des stratégies de filtrage du courrier indésirable, voir [Configurer vos stratégies de filtrage du courrier indésirable.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="6bfce-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
