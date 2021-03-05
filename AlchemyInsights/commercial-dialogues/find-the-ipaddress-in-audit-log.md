---
title: Rechercher l’adresse IP dans le journal d’audit
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464705"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="7da85-102">Rechercher l’adresse IP dans le journal d’audit</span><span class="sxs-lookup"><span data-stu-id="7da85-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="7da85-103">L’adresse IP qui correspond à une activité effectuée par un utilisateur ou un administrateur est affichée dans les journaux d’audit.</span><span class="sxs-lookup"><span data-stu-id="7da85-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="7da85-104">Les informations client sont également enregistrées.</span><span class="sxs-lookup"><span data-stu-id="7da85-104">The client information is also logged.</span></span> <span data-ttu-id="7da85-105">Voici comment identifier l’adresse IP :</span><span class="sxs-lookup"><span data-stu-id="7da85-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="7da85-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="7da85-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="7da85-107">Sélectionnez **recherche**  >  **[dans le journal d’audit de recherche.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="7da85-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7da85-108">Si un avis vous demande d’activer l’audit, allez de l’avant et l’activer maintenant.</span><span class="sxs-lookup"><span data-stu-id="7da85-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="7da85-109">Si cette fonctionnalité n’est pas activée, les résultats de la recherche ne pourront pas tirer les données des dates précédentes.</span><span class="sxs-lookup"><span data-stu-id="7da85-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="7da85-110">Si une activité spécifique vous intéresse, sélectionnez-la dans la liste **Activités** . Sinon, par défaut, toutes les activités sont renvoyées pour l’utilisateur sélectionné.</span><span class="sxs-lookup"><span data-stu-id="7da85-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="7da85-111">Notez que certaines activités peuvent ne pas être disponibles pour la sélection dans le menu **Activités** ; toutefois, ces éléments d’audit sont renvoyés si **l’option Afficher** les résultats de toutes les activités est sélectionnée (paramètre par défaut).</span><span class="sxs-lookup"><span data-stu-id="7da85-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="7da85-112">Spécifiez la plage de dates et, dans le champ **Utilisateurs,** sélectionnez le nom d’utilisateur de l’utilisateur que vous souhaitez examiner.</span><span class="sxs-lookup"><span data-stu-id="7da85-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="7da85-113">Sélectionnez **Rechercher.**</span><span class="sxs-lookup"><span data-stu-id="7da85-113">Select **Search**.</span></span> <span data-ttu-id="7da85-114">Les activités apparaissent sous **Résultats**.</span><span class="sxs-lookup"><span data-stu-id="7da85-114">The activities appear under **Results**.</span></span> <span data-ttu-id="7da85-115">Vous pouvez voir l’adresse IP de chaque activité.</span><span class="sxs-lookup"><span data-stu-id="7da85-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="7da85-116">Pour afficher les détails, sélectionnez une activité, puis sélectionnez **Plus d’informations.**</span><span class="sxs-lookup"><span data-stu-id="7da85-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="7da85-117">Pour en savoir plus, consultez la recherche dans le journal [d’audit Office 365 pour résoudre les problèmes de scénarios courants.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="7da85-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>