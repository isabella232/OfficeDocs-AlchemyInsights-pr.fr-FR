---
title: Exemple de stratégie de pièces jointes sécurisées Microsoft Defender pour Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736748"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="0a720-102">Exemple de stratégie de pièces jointes sécurisées Microsoft Defender pour Office 365</span><span class="sxs-lookup"><span data-stu-id="0a720-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="0a720-103">Ces paramètres activent une stratégie appelée *Aucun* délai qui fournit les messages immédiatement, puis réattaque les pièces jointes après leur analyse :</span><span class="sxs-lookup"><span data-stu-id="0a720-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="0a720-104">**Nom**: aucun délai</span><span class="sxs-lookup"><span data-stu-id="0a720-104">**Name**: No delays</span></span>
- <span data-ttu-id="0a720-105">**Description**: fournit les messages immédiatement et réattaque les pièces jointes après analyse.</span><span class="sxs-lookup"><span data-stu-id="0a720-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="0a720-106">**Réponse**: sélectionnez **l’option Remise** dynamique.</span><span class="sxs-lookup"><span data-stu-id="0a720-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="0a720-107">Pour plus d’informations, [voir Remise dynamique dans les stratégies de pièces jointes sécurisées.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="0a720-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="0a720-108">**Section** Rediriger les pièces jointes : sélectionnez l’option Activer la **redirection,** puis entrez l’adresse e-mail de votre administrateur général Microsoft 365, administrateur de sécurité ou analyste de sécurité qui étudiera les pièces jointes malveillantes.</span><span class="sxs-lookup"><span data-stu-id="0a720-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="0a720-109">**Section Appliqué à** : **Sélectionnez le domaine du destinataire,** puis sélectionnez votre domaine.</span><span class="sxs-lookup"><span data-stu-id="0a720-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="0a720-110">Sélectionnez **Ajouter,** puis **OK.**</span><span class="sxs-lookup"><span data-stu-id="0a720-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="0a720-111">Une fois que vous avez terminé, sélectionnez **Enregistrer.**</span><span class="sxs-lookup"><span data-stu-id="0a720-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="0a720-112">Pour plus d’informations, [voir Pièces jointes sécurisées dans Microsoft Defender pour Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="0a720-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>