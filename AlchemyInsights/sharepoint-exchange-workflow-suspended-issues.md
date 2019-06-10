---
title: Prise en main de SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770561"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="31978-102">Flux de travail dans SharePoint</span><span class="sxs-lookup"><span data-stu-id="31978-102">Workflows in SharePoint</span></span>

<span data-ttu-id="31978-103">Si les flux de travail SharePoint n’envoient pas d’e-mails, il se peut que votre organisation ait rencontré des limites d’expéditeurs Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="31978-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="31978-104">Le message d’erreur «le flux de travail est suspendu» peut se produire si vous avez l’un des éléments suivants:</span><span class="sxs-lookup"><span data-stu-id="31978-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="31978-105">Vous disposez d’un flux de travail dans SharePoint Online qui utilise le type de plateforme de flux de travail SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="31978-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="31978-106">Le flux de travail est configuré pour envoyer un message électronique personnalisé à plus de 200 utilisateurs à la fois, plus de 10 000 destinataires par jour ou plus de 30 messages par minute.</span><span class="sxs-lookup"><span data-stu-id="31978-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="31978-107">Lorsque vous exécutez le flux de travail, le message électronique n’est pas envoyé et vous remarquez le message d’erreur, le statut Internal est défini sur suspendu ou impossible d’envoyer à un destinataire est affiché.</span><span class="sxs-lookup"><span data-stu-id="31978-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="31978-108">Pour plus d’informations, reportez-vous à l' [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)suivant.</span><span class="sxs-lookup"><span data-stu-id="31978-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

