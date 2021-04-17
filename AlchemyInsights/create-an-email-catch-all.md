---
title: Créer un e-mail catch all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816198"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="80001-102">Créer un e-mail catch all</span><span class="sxs-lookup"><span data-stu-id="80001-102">Create an email catch all</span></span>

<span data-ttu-id="80001-103">L’utilisation d’un « catch all » est fortement déconseillée.</span><span class="sxs-lookup"><span data-stu-id="80001-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="80001-104">Il est préférable de renvoyer une nouvelle fois à l’expéditeur pour que les expéditeurs sachent que leur message n’a pas pu être remis comme traité afin qu’ils prennent des mesures.</span><span class="sxs-lookup"><span data-stu-id="80001-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="80001-105">Vous pouvez également limiter la boîte aux lettres surveillée pour qu’elle capture uniquement les adresses de messagerie auparavant valides.</span><span class="sxs-lookup"><span data-stu-id="80001-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="80001-106">Toute boîte aux lettres « catch » reçoit une grande partie du courrier indésirable et peut finir par remplir si elle n’est pas surveillée de près.</span><span class="sxs-lookup"><span data-stu-id="80001-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="80001-107">(Il existe des limites de réception.)</span><span class="sxs-lookup"><span data-stu-id="80001-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="80001-108">Si vous décidez de continuer, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="80001-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="80001-109">Créez un groupe de distribution dynamique & inclure « Tous les types de destinataires ».</span><span class="sxs-lookup"><span data-stu-id="80001-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="80001-110">Créez une boîte aux lettres dédiée pour capturer les messages électroniques, par exemple, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="80001-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="80001-111">Pour le domaine spécifique, définissez DomainType sur « InternalRelay ».</span><span class="sxs-lookup"><span data-stu-id="80001-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="80001-112">Si vous supprimez ultérieurement le catch all, n’oubliez pas de définir le domaine sur Faisant autorité.</span><span class="sxs-lookup"><span data-stu-id="80001-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="80001-113">Créez une règle de transport de flux de messagerie comme suit :</span><span class="sxs-lookup"><span data-stu-id="80001-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="80001-114">Si l’expéditeur est « en dehors de l’organisation »</span><span class="sxs-lookup"><span data-stu-id="80001-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="80001-115">Rediriger le message vers Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="80001-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="80001-116">Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)</span><span class="sxs-lookup"><span data-stu-id="80001-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="80001-117">Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique</span><span class="sxs-lookup"><span data-stu-id="80001-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
