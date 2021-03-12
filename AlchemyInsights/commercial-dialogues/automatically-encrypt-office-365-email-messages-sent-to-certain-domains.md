---
title: Chiffrer automatiquement les messages électroniques Office 365 envoyés à certains domaines
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736780"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="9db33-102">Chiffrer automatiquement les messages électroniques Office 365 envoyés à certains domaines</span><span class="sxs-lookup"><span data-stu-id="9db33-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="9db33-103">Dans le Centre [d’administration Exchange,](https://outlook.office365.com/ecp/)sélectionnez **flux de messagerie > règles.**</span><span class="sxs-lookup"><span data-stu-id="9db33-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9db33-104">Cliquez sur **l’icône Nouveau (+),** puis cliquez sur Appliquer le chiffrement de messages **Office 365** et la protection des droits aux messages.</span><span class="sxs-lookup"><span data-stu-id="9db33-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9db33-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="9db33-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="9db33-106">In **Apply this rule if**, choose The recipient > domain **is**.</span><span class="sxs-lookup"><span data-stu-id="9db33-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="9db33-107">Entrez le nom du domaine, tel que **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="9db33-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="9db33-108">Cliquez sur **l’icône Ajouter (+),** puis sur **OK.**</span><span class="sxs-lookup"><span data-stu-id="9db33-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="9db33-109">En plus du **champ Faire le champ** Suivant, cliquez sur Sélectionner **un**.</span><span class="sxs-lookup"><span data-stu-id="9db33-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="9db33-110">Dans le menu **déroulant du modèle RMS,** sélectionnez **Chiffrer,** puis cliquez sur **OK.**</span><span class="sxs-lookup"><span data-stu-id="9db33-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9db33-111">(Si cette option n’est pas disponible, cela signifie que votre plan n’inclut pas le chiffrement automatique.</span><span class="sxs-lookup"><span data-stu-id="9db33-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9db33-112">Mais vous pouvez l’ajouter !)</span><span class="sxs-lookup"><span data-stu-id="9db33-112">But you can add it!)</span></span>
9. <span data-ttu-id="9db33-113">Choisissez n’importe quelle sélection facultative (dans une liste de sélections facultatives que vous pouvez effectuer à ce stade, dont la plupart peuvent être laissées avec le paramètre par défaut par souci de simplicité).</span><span class="sxs-lookup"><span data-stu-id="9db33-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9db33-114">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="9db33-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9db33-115">Vous pouvez toujours revenir et modifier cette règle ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="9db33-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9db33-116">Pour plus d’informations sur la création de règles de chiffrement, voir Définir des règles de flux de messagerie pour chiffrer les [messages électroniques dans Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="9db33-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>