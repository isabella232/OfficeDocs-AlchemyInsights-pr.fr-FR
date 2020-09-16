---
title: Plusieurs objets ont la même adresse de courrier comme identité
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724613"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="49c5a-102">Plusieurs objets ont la même adresse de courrier comme identité</span><span class="sxs-lookup"><span data-stu-id="49c5a-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="49c5a-103">**Objets multiples**</span><span class="sxs-lookup"><span data-stu-id="49c5a-103">**Multiple objects**</span></span>

<span data-ttu-id="49c5a-104">L’une des raisons les plus fréquentes de cette erreur est de ne pas pouvoir acheminer correctement une demande Outlook Web Access en présence de plusieurs objets ayant la même adresse de messagerie que l’identité.</span><span class="sxs-lookup"><span data-stu-id="49c5a-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="49c5a-105">Pour rechercher ces objets, exécutez les commandes suivantes :</span><span class="sxs-lookup"><span data-stu-id="49c5a-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="49c5a-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="49c5a-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="49c5a-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="49c5a-107">· Get-User <email address></span></span>

<span data-ttu-id="49c5a-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="49c5a-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="49c5a-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="49c5a-109">· Get-Contact <email address></span></span>

<span data-ttu-id="49c5a-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="49c5a-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="49c5a-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="49c5a-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="49c5a-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="49c5a-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="49c5a-113">Pour résoudre le problème, supprimez plusieurs objets avec la même identité de courrier et assurez-vous qu’il existe un objet unique avec l’identité de courrier spécifique et que son type de destinataire est UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="49c5a-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="49c5a-114">**La même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public**</span><span class="sxs-lookup"><span data-stu-id="49c5a-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="49c5a-115">Une autre cause est que la même adresse est utilisée pour les boîtes aux lettres d’entreprise et les boîtes aux lettres grand public.</span><span class="sxs-lookup"><span data-stu-id="49c5a-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="49c5a-116">Dans ce cas, l’utilisateur doit changer d’alias de consommateur principal jusqu’à ce que le café prenne en charge ce scénario.</span><span class="sxs-lookup"><span data-stu-id="49c5a-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="49c5a-117">Il s’agit d’une erreur permanente qui ne disparaît pas sans intervention.</span><span class="sxs-lookup"><span data-stu-id="49c5a-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="49c5a-118">Pour plus d’informations, consultez [Modifier l’adresse de courrier ou le numéro de téléphone de votre compte Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="49c5a-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>