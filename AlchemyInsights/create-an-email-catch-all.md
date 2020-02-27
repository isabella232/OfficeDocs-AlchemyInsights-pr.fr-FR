---
title: Créer un e-mail attraper tout
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286108"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="2cbad-102">Créer un e-mail attraper tout</span><span class="sxs-lookup"><span data-stu-id="2cbad-102">Create an email catch all</span></span>

<span data-ttu-id="2cbad-103">L’utilisation d’une capture tout est fortement déconseillée.</span><span class="sxs-lookup"><span data-stu-id="2cbad-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="2cbad-104">Il est préférable de renvoyer un message à l’expéditeur pour informer les expéditeurs qu’ils n’ont pas pu être remis comme adressés afin qu’ils puissent agir.</span><span class="sxs-lookup"><span data-stu-id="2cbad-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="2cbad-105">Vous pouvez également limiter la boîte aux lettres surveillée afin d’intercepter uniquement les adresses de messagerie valides précédemment.</span><span class="sxs-lookup"><span data-stu-id="2cbad-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="2cbad-106">Toute boîte aux lettres peut recevoir une grande quantité de courrier indésirable et éventuellement remplir si elle n’est pas soigneusement surveillée.</span><span class="sxs-lookup"><span data-stu-id="2cbad-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="2cbad-107">(Il existe des limites de réception.)</span><span class="sxs-lookup"><span data-stu-id="2cbad-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="2cbad-108">Si vous décidez de procéder, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="2cbad-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="2cbad-109">Créez un groupe de distribution dynamique & inclure « tous les types de destinataires ».</span><span class="sxs-lookup"><span data-stu-id="2cbad-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="2cbad-110">Créez une boîte aux lettres dédiée pour intercepter des courriers électroniques, par exemple, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="2cbad-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="2cbad-111">Pour le domaine spécifique, définissez DomainType sur « InternalRelay ».</span><span class="sxs-lookup"><span data-stu-id="2cbad-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="2cbad-112">Si vous supprimez par la suite le paramètre catch tout, veillez à redéfinir le domaine sur faisant autorité.</span><span class="sxs-lookup"><span data-stu-id="2cbad-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="2cbad-113">Créez une règle de transport de flux de flux comme suit :</span><span class="sxs-lookup"><span data-stu-id="2cbad-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="2cbad-114">Si l’expéditeur est « à l’extérieur de l’Organisation »</span><span class="sxs-lookup"><span data-stu-id="2cbad-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="2cbad-115">Rediriger le message vers Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="2cbad-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="2cbad-116">Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)</span><span class="sxs-lookup"><span data-stu-id="2cbad-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="2cbad-117">Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique</span><span class="sxs-lookup"><span data-stu-id="2cbad-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
