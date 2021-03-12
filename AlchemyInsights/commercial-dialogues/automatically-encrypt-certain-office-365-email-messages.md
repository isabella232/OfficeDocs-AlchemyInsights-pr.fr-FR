---
title: Chiffrer automatiquement certains messages électroniques Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736827"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="a14cc-102">Chiffrer automatiquement certains messages électroniques Office 365</span><span class="sxs-lookup"><span data-stu-id="a14cc-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="a14cc-103">Vous pouvez chiffrer automatiquement les messages que les utilisateurs envoient à certaines personnes ou organisations externes.</span><span class="sxs-lookup"><span data-stu-id="a14cc-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="a14cc-104">Pour ce faire, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a14cc-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="a14cc-105">Dans le Centre [d’administration Exchange,](https://outlook.office365.com/ecp/)sélectionnez **flux de messagerie > règles.**</span><span class="sxs-lookup"><span data-stu-id="a14cc-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a14cc-106">Cliquez sur **l’icône Nouveau (+),** puis cliquez sur Appliquer le chiffrement de messages **Office 365** et la protection des droits aux messages.</span><span class="sxs-lookup"><span data-stu-id="a14cc-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a14cc-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="a14cc-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="a14cc-108">In **Apply this rule if**, choose The recipient > is this **person**.</span><span class="sxs-lookup"><span data-stu-id="a14cc-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="a14cc-109">Dans la **fenêtre Sélectionner des** membres, sélectionnez le nom de la personne à qui la règle de chiffrement doit s’appliquer, puis cliquez sur **Ajouter.**</span><span class="sxs-lookup"><span data-stu-id="a14cc-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="a14cc-110">Lorsque vous avez terminé d’ajouter des utilisateurs, cliquez **sur OK.**</span><span class="sxs-lookup"><span data-stu-id="a14cc-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="a14cc-111">En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**.</span><span class="sxs-lookup"><span data-stu-id="a14cc-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="a14cc-112">Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.**</span><span class="sxs-lookup"><span data-stu-id="a14cc-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a14cc-113">(Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique.</span><span class="sxs-lookup"><span data-stu-id="a14cc-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a14cc-114">Mais vous pouvez l’ajouter !)</span><span class="sxs-lookup"><span data-stu-id="a14cc-114">But you can add it!)</span></span>
9. <span data-ttu-id="a14cc-115">Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut par souci de simplicité).</span><span class="sxs-lookup"><span data-stu-id="a14cc-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a14cc-116">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="a14cc-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a14cc-117">Vous pouvez toujours revenir et modifier cette règle ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="a14cc-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a14cc-118">Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour chiffrer les messages électroniques [dans Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a14cc-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

