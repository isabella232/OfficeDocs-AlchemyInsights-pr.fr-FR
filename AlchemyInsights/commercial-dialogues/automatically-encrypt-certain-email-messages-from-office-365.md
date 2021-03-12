---
title: Chiffrer automatiquement certains messages électroniques à partir d’Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736828"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="12cf5-102">Chiffrer automatiquement certains messages électroniques à partir d’Office 365</span><span class="sxs-lookup"><span data-stu-id="12cf5-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="12cf5-103">Dans le Centre [d’administration Exchange,](https://outlook.office365.com/ecp/)sélectionnez **flux de messagerie > règles.**</span><span class="sxs-lookup"><span data-stu-id="12cf5-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="12cf5-104">Cliquez sur **l’icône Nouveau (+),** puis cliquez sur Appliquer le chiffrement de messages **Office 365** et la protection des droits aux messages.</span><span class="sxs-lookup"><span data-stu-id="12cf5-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="12cf5-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span><span class="sxs-lookup"><span data-stu-id="12cf5-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="12cf5-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span><span class="sxs-lookup"><span data-stu-id="12cf5-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="12cf5-107">En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**.</span><span class="sxs-lookup"><span data-stu-id="12cf5-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="12cf5-108">Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.**</span><span class="sxs-lookup"><span data-stu-id="12cf5-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="12cf5-109">(Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique.</span><span class="sxs-lookup"><span data-stu-id="12cf5-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="12cf5-110">Mais vous pouvez l’ajouter !)</span><span class="sxs-lookup"><span data-stu-id="12cf5-110">But you can add it!)</span></span>
7. <span data-ttu-id="12cf5-111">Cochez **la case Auditer** cette règle avec le niveau de gravité, puis sélectionnez le niveau souhaité.</span><span class="sxs-lookup"><span data-stu-id="12cf5-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="12cf5-112">Si votre entreprise a des obligations contractuelles d’envoyer tous les e-mails chiffrés, je vous recommande de définir le niveau sur **Élevé**.</span><span class="sxs-lookup"><span data-stu-id="12cf5-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="12cf5-113">Sous **Choisir un modèle pour cette règle,** cliquez sur **Appliquer.**</span><span class="sxs-lookup"><span data-stu-id="12cf5-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="12cf5-114">Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut par souci de simplicité).</span><span class="sxs-lookup"><span data-stu-id="12cf5-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="12cf5-115">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="12cf5-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="12cf5-116">Vous pouvez toujours revenir et modifier cette règle ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="12cf5-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="12cf5-117">Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour chiffrer les [messages électroniques dans Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="12cf5-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

