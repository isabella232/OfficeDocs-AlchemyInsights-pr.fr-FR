---
title: Créer un e-mail attraper tout
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712984"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c7dd1-102">Créer un e-mail attraper tout</span><span class="sxs-lookup"><span data-stu-id="c7dd1-102">Create an email catch all</span></span>

<span data-ttu-id="c7dd1-103">L’utilisation d’une capture tout est fortement déconseillée.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c7dd1-104">Il est préférable de renvoyer un message à l’expéditeur pour informer les expéditeurs qu’ils n’ont pas pu être remis comme adressés afin qu’ils puissent agir.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c7dd1-105">Vous pouvez également limiter la boîte aux lettres surveillée afin d’intercepter uniquement les adresses de messagerie valides précédemment.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c7dd1-106">Toute boîte aux lettres peut recevoir une grande quantité de courrier indésirable et éventuellement remplir si elle n’est pas soigneusement surveillée.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c7dd1-107">(Il existe des limites de réception.)</span><span class="sxs-lookup"><span data-stu-id="c7dd1-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c7dd1-108">Si vous décidez de procéder, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="c7dd1-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c7dd1-109">Créez un groupe de distribution dynamique & inclure « tous les types de destinataires ».</span><span class="sxs-lookup"><span data-stu-id="c7dd1-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c7dd1-110">Créez une boîte aux lettres dédiée pour intercepter des courriers électroniques, par exemple, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c7dd1-111">Pour le domaine spécifique, définissez DomainType sur « InternalRelay ».</span><span class="sxs-lookup"><span data-stu-id="c7dd1-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c7dd1-112">Si vous supprimez par la suite le paramètre catch tout, veillez à redéfinir le domaine sur faisant autorité.</span><span class="sxs-lookup"><span data-stu-id="c7dd1-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c7dd1-113">Créez une règle de transport de flux de flux comme suit :</span><span class="sxs-lookup"><span data-stu-id="c7dd1-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c7dd1-114">Si l’expéditeur est « à l’extérieur de l’Organisation »</span><span class="sxs-lookup"><span data-stu-id="c7dd1-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c7dd1-115">Rediriger le message vers Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="c7dd1-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c7dd1-116">Sauf si le destinataire est membre de allusers@domain.com (le groupe de distribution contient tous les membres)</span><span class="sxs-lookup"><span data-stu-id="c7dd1-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c7dd1-117">Vérifier que les nouvelles boîtes aux lettres sont ajoutées au groupe de distribution dynamique</span><span class="sxs-lookup"><span data-stu-id="c7dd1-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
