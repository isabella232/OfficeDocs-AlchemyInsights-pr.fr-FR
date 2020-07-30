---
title: Plusieurs objets ont la même adresse de courrier comme identité
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431405"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="7758e-102">Plusieurs objets ont la même adresse de courrier comme identité</span><span class="sxs-lookup"><span data-stu-id="7758e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="7758e-103">**Objets multiples**</span><span class="sxs-lookup"><span data-stu-id="7758e-103">**Multiple objects**</span></span>

<span data-ttu-id="7758e-104">L’une des raisons les plus fréquentes de cette erreur est de ne pas pouvoir acheminer correctement une demande Outlook Web Access en présence de plusieurs objets ayant la même adresse de messagerie que l’identité.</span><span class="sxs-lookup"><span data-stu-id="7758e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="7758e-105">Pour rechercher ces objets, exécutez les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="7758e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="7758e-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="7758e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="7758e-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="7758e-107">· Get-User <email address></span></span>

<span data-ttu-id="7758e-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="7758e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="7758e-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="7758e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="7758e-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="7758e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="7758e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="7758e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="7758e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="7758e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="7758e-113">Pour résoudre le problème, supprimez plusieurs objets avec la même identité de courrier et assurez-vous qu’il existe un objet unique avec l’identité de courrier spécifique et que son type de destinataire est UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="7758e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="7758e-114">**La même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public**</span><span class="sxs-lookup"><span data-stu-id="7758e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="7758e-115">Une autre cause est que la même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public.</span><span class="sxs-lookup"><span data-stu-id="7758e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="7758e-116">Dans ce cas, l’utilisateur doit changer d’alias de consommateur principal jusqu’à ce que le café prenne en charge ce scénario.</span><span class="sxs-lookup"><span data-stu-id="7758e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="7758e-117">Il s’agit d’une erreur permanente qui ne disparaît pas sans intervention.</span><span class="sxs-lookup"><span data-stu-id="7758e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="7758e-118">Pour plus d’informations, consultez [Modifier l’adresse de courrier ou le numéro de téléphone de votre compte Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="7758e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>