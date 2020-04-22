---
title: Identifier l’activité des règles de boîte de réception dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716422"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="31f7a-102">Identifier l’activité des règles de boîte de réception dans les journaux d’audit</span><span class="sxs-lookup"><span data-stu-id="31f7a-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="31f7a-103">Vous pouvez utiliser la recherche dans le journal d’audit du centre de sécurité & de Microsoft 365 pour afficher les événements de règles de boîte de réception (création, modification et suppression de règles de boîte de réception).</span><span class="sxs-lookup"><span data-stu-id="31f7a-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="31f7a-104">Connectez-vous au [Centre de conformité & Microsoft 365 Security](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="31f7a-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="31f7a-105">Accédez à la page de**recherche du journal d’audit** de la **recherche** > .</span><span class="sxs-lookup"><span data-stu-id="31f7a-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="31f7a-106">Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** .</span><span class="sxs-lookup"><span data-stu-id="31f7a-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="31f7a-107">Sous **activités de boîte aux lettres Exchange**, vérifiez que le champ **activités** est défini sur **nouveau-InboxRule créer/modifier/activer/désactiver la règle de boîte de réception**.</span><span class="sxs-lookup"><span data-stu-id="31f7a-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="31f7a-108">Cliquez sur **Rechercher**.</span><span class="sxs-lookup"><span data-stu-id="31f7a-108">Click **Search**.</span></span>

<span data-ttu-id="31f7a-109">Dans les résultats, sélectionnez un enregistrement d’audit.</span><span class="sxs-lookup"><span data-stu-id="31f7a-109">In the results, select an audit record.</span></span> <span data-ttu-id="31f7a-110">Dans la fenêtre mobile des détails, cliquez sur **informations supplémentaires**.</span><span class="sxs-lookup"><span data-stu-id="31f7a-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="31f7a-111">Les informations sur les paramètres des règles de boîte de réception sont affichées dans le champ **paramètres** .</span><span class="sxs-lookup"><span data-stu-id="31f7a-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="31f7a-112">Pour plus d’informations, consultez [la rubrique déterminer si un utilisateur a créé une règle de boîte de réception](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="31f7a-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
