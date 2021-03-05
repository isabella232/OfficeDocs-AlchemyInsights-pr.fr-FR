---
title: Lire les journaux d’audit pour les événements supprimés
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464602"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="fe341-102">Lire les journaux d’audit pour les événements supprimés</span><span class="sxs-lookup"><span data-stu-id="fe341-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="fe341-103">Voici comment faire :</span><span class="sxs-lookup"><span data-stu-id="fe341-103">Here's how to do this:</span></span>

1. <span data-ttu-id="fe341-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="fe341-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="fe341-105">Sélectionnez **recherche**  >  [**dans le journal d’audit de recherche.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="fe341-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="fe341-106">Si une notification vous demande d’activer la fonctionnalité, allez de l’avant et l’activer maintenant.</span><span class="sxs-lookup"><span data-stu-id="fe341-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="fe341-107">Si la fonctionnalité n’est pas désactivée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.</span><span class="sxs-lookup"><span data-stu-id="fe341-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="fe341-108">Sélectionnez **Activités,** puis recherchez les activités de **boîte aux lettres Exchange.**</span><span class="sxs-lookup"><span data-stu-id="fe341-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="fe341-109">Sélectionnez **les messages supprimés** du dossier Éléments supprimés et les **options du** dossier Éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="fe341-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="fe341-110">Lorsque vous avez terminé, cliquez en dehors du volet pour réduire le **volet** Activités.</span><span class="sxs-lookup"><span data-stu-id="fe341-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="fe341-111">Spécifiez la plage de  dates, puis dans la zone Utilisateurs, sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner.</span><span class="sxs-lookup"><span data-stu-id="fe341-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="fe341-112">Vous pouvez sélectionner plusieurs utilisateurs à la fois.</span><span class="sxs-lookup"><span data-stu-id="fe341-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="fe341-113">Sélectionnez **Rechercher.**</span><span class="sxs-lookup"><span data-stu-id="fe341-113">Select **Search**.</span></span> <span data-ttu-id="fe341-114">Les activités apparaissent sous **Résultats**.</span><span class="sxs-lookup"><span data-stu-id="fe341-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="fe341-115">Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.**</span><span class="sxs-lookup"><span data-stu-id="fe341-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="fe341-116">Des informations supplémentaires sur l’élément supprimé, telles que la ligne d’objet et l’emplacement de l’élément lors de sa suppression, sont affichées dans le champ **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="fe341-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="fe341-117">Vous ne pouvez pas restaurer les éléments supprimés à l’aide de la fonctionnalité journal d’audit.</span><span class="sxs-lookup"><span data-stu-id="fe341-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="fe341-118">Pour restaurer des éléments supprimés, voir Récupérer les éléments supprimés ou [le courrier électronique dans Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="fe341-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="fe341-119">Pour en savoir plus, consultez la recherche [dans le journal d’audit Office 365 pour résoudre les problèmes de scénarios courants.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="fe341-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
