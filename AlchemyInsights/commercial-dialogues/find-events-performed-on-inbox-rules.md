---
title: Rechercher des événements effectués sur des règles de boîte de réception
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464702"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="89196-102">Rechercher des événements effectués sur des règles de boîte de réception</span><span class="sxs-lookup"><span data-stu-id="89196-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="89196-103">Lorsque des règles de boîte de réception sont créées, modifiées ou supprimées, les événements sont enregistrés dans le journal d’audit.</span><span class="sxs-lookup"><span data-stu-id="89196-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="89196-104">Voici comment les examiner :</span><span class="sxs-lookup"><span data-stu-id="89196-104">Here's how to review them:</span></span>

1. <span data-ttu-id="89196-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="89196-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="89196-106">Sélectionnez Rechercher > recherche dans le journal d’audit.</span><span class="sxs-lookup"><span data-stu-id="89196-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="89196-107">Si un avis vous demande d’activer l’audit, allez de l’avant et l’activer maintenant.</span><span class="sxs-lookup"><span data-stu-id="89196-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="89196-108">Si cette fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.</span><span class="sxs-lookup"><span data-stu-id="89196-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="89196-109">Sélectionnez le champ Activités et recherchez les activités de boîte aux lettres Exchange, puis sélectionnez New-InboxRule créer une règle de boîte de réception à partir d’Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="89196-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="89196-110">Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le volet Activités.</span><span class="sxs-lookup"><span data-stu-id="89196-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="89196-111">Spécifiez la plage de dates, puis dans le champ Utilisateurs, sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner.</span><span class="sxs-lookup"><span data-stu-id="89196-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="89196-112">Vous pouvez sélectionner plusieurs utilisateurs à la fois.</span><span class="sxs-lookup"><span data-stu-id="89196-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="89196-113">Sélectionnez Rechercher.</span><span class="sxs-lookup"><span data-stu-id="89196-113">Select Search.</span></span> <span data-ttu-id="89196-114">Les activités apparaissent sous Résultats.</span><span class="sxs-lookup"><span data-stu-id="89196-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="89196-115">Pour afficher les détails, sélectionnez une activité, puis sélectionnez Plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="89196-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="89196-116">Sous la section Paramètres, vous pouvez voir le nom de la règle, les conditions définies et les actions que la règle va prendre.</span><span class="sxs-lookup"><span data-stu-id="89196-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="89196-117">Pour en savoir plus, consultez la recherche dans le journal d’audit Office 365 pour résoudre les problèmes de scénarios courants.</span><span class="sxs-lookup"><span data-stu-id="89196-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>