---
title: Limite de messagerie quotidienne dépassée. Le flux de travail est suspendu.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580331"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="54984-103">Limite de messagerie quotidienne dépassée.</span><span class="sxs-lookup"><span data-stu-id="54984-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="54984-104">Le flux de travail est suspendu.</span><span class="sxs-lookup"><span data-stu-id="54984-104">Workflow is suspended.</span></span>

<span data-ttu-id="54984-105">Cette erreur peut être reçue dans les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="54984-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="54984-106">Vous disposez d’un flux de travail dans SharePoint Online qui utilise le type de plateforme de flux de travail SharePoint 2010 ou SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="54984-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="54984-107">Le flux de travail est configuré pour envoyer un message électronique personnalisé à plus de 200 utilisateurs à la fois, plus de 10 000 destinataires par jour ou plus de 30 messages par minute.</span><span class="sxs-lookup"><span data-stu-id="54984-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="54984-108">Lorsque vous exécutez le flux de travail, le message électronique n’est pas envoyé et vous remarquez le comportement suivant :</span><span class="sxs-lookup"><span data-stu-id="54984-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="54984-109">Pour un flux de travail qui utilise le type de plateforme SharePoint 2013, accédez à la page **État du flux de travail** .</span><span class="sxs-lookup"><span data-stu-id="54984-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="54984-110">Dans la page État du flux de travail, le **statut interne** est défini sur **démarré**, et la bulle d’informations affiche **Impossible d’envoyer à un destinataire**.</span><span class="sxs-lookup"><span data-stu-id="54984-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="54984-111">Pour contourner ce problème, configurez votre flux de travail pour qu’il envoie des messages électroniques sans dépasser les limites de l' [expéditeur Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="54984-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="54984-112">Par exemple, utilisez une pause dans le flux de travail, envoyez l’e-mail à un groupe de sécurité Microsoft 365, à un groupe de distribution ou à un groupe de sécurité à extension messagerie, ou envoyez le message à moins de 200 destinataires à la fois.</span><span class="sxs-lookup"><span data-stu-id="54984-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="54984-113">Pour plus d’informations, consultez l' [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)suivant.</span><span class="sxs-lookup"><span data-stu-id="54984-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="54984-114">Rubriques connexes</span><span class="sxs-lookup"><span data-stu-id="54984-114">Related topics</span></span>
- [<span data-ttu-id="54984-115">Créer un flux</span><span class="sxs-lookup"><span data-stu-id="54984-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="54984-116">SharePoint et flux</span><span class="sxs-lookup"><span data-stu-id="54984-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 