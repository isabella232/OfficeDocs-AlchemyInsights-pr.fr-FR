---
title: " S/MIME dans Outlook sur le web"
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764870"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="bf7f7-102">Chiffrer les messages électroniques dans Outlook</span><span class="sxs-lookup"><span data-stu-id="bf7f7-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="bf7f7-103">Le chiffrement de messages Microsoft 365 est basé sur Microsoft Azure Rights Management (Azure RMS), qui fait partie d’Azure information protection.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="bf7f7-104">Si votre abonnement inclut Azure Rights Management ou Azure information protection, **il n’est pas nécessaire d’effectuer des actions pour activer ou activer manuellement** le service gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="bf7f7-105">En fonction des commentaires des clients, nous n’allons plus activer les règles de flux de messagerie Exchange pour chiffrer automatiquement les messages électroniques sortants contenant certains types d’informations sensibles dans votre client par défaut.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="bf7f7-106">Au lieu de cela, nous fournissons des instructions détaillées pour vous permettre de le faire.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="bf7f7-107">Pour plus d’informations sur la création d’une règle de transport pour chiffrer des informations sensibles, consultez [cet article](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="bf7f7-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="bf7f7-108">Si vous utilisez Outlook sur le Web (anciennement **owa**) : lors de la composition d’un message électronique, cliquez simplement sur **protéger** dans OWA.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="bf7f7-109">Cette action s’applique à l’autorisation « ne pas transférer ».</span><span class="sxs-lookup"><span data-stu-id="bf7f7-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="bf7f7-110">Cliquez sur **modifier l’autorisation** et sélectionnez **chiffrer** pour uniquement chiffrer le message.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="bf7f7-111">Si vous utilisez le **client Outlook**: pour envoyer un message chiffré à partir d’Outlook 2013 ou 2016, ou Outlook 2016 pour Mac, sélectionnez **options** > **autorisations**, puis sélectionnez l’option de protection dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="bf7f7-112">Pour **chiffrer automatiquement tous les messages électroniques** envoyés à certains destinataires ou organisations partenaires externes, vous devez créer une règle de transport de flux de messagerie dans le centre d’administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf7f7-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="bf7f7-113">Des instructions détaillées sont fournies dans [cet article de support technique](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="bf7f7-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

