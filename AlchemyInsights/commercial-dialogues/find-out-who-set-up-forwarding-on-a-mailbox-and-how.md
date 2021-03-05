---
title: Savoir qui a installé le forwarding sur une boîte aux lettres et comment
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464614"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="ed576-102">Savoir qui a installé le forwarding sur une boîte aux lettres et comment</span><span class="sxs-lookup"><span data-stu-id="ed576-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="ed576-103">Si le forwarding externe a été définie sur une boîte aux lettres, l’activité est auditée dans le cadre Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="ed576-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="ed576-104">Voici comment rechercher l’activité dans le journal d’audit :</span><span class="sxs-lookup"><span data-stu-id="ed576-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="ed576-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ed576-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ed576-106">Sélectionnez **recherche** >  **dans le journal d’audit de recherche.**</span><span class="sxs-lookup"><span data-stu-id="ed576-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ed576-107">Si un avis vous demande d’activer l’audit, allez de l’avant et l’activer maintenant.</span><span class="sxs-lookup"><span data-stu-id="ed576-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ed576-108">Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.</span><span class="sxs-lookup"><span data-stu-id="ed576-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ed576-109">Assurez-vous **que le champ Activités** est définie sur Afficher les résultats pour toutes les **activités** (valeur par défaut).</span><span class="sxs-lookup"><span data-stu-id="ed576-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="ed576-110">Spécifiez la plage de dates.</span><span class="sxs-lookup"><span data-stu-id="ed576-110">Specify the date range.</span></span> <span data-ttu-id="ed576-111">Vous n’avez pas besoin de spécifier un nom d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ed576-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="ed576-112">Sélectionnez **Rechercher.**</span><span class="sxs-lookup"><span data-stu-id="ed576-112">Select **Search**.</span></span> <span data-ttu-id="ed576-113">Les activités apparaissent sous **Résultats**.</span><span class="sxs-lookup"><span data-stu-id="ed576-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="ed576-114">Sélectionnez **Résultats du** filtre, puis entrez **Set-mailbox** dans le champ **De** filtre Activité.</span><span class="sxs-lookup"><span data-stu-id="ed576-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="ed576-115">Cette action renvoie toutes **les activités Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="ed576-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="ed576-116">Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.**</span><span class="sxs-lookup"><span data-stu-id="ed576-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="ed576-117">Sous **Paramètres,** vous pouvez voir l’adresse de messagerie de forwarding qui a été définie sur la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed576-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="ed576-118">UserID **représente** l’utilisateur qui a installé le forwarding externe sur la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed576-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="ed576-119">Pour en savoir plus, consultez la recherche [dans le journal d’audit Office 365 pour résoudre les problèmes de scénarios courants.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="ed576-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>