---
title: Identifier l’activité des règles de boîte de réception dans les journaux d’audit
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755036"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="f40c4-102">Identifier l’activité des règles de boîte de réception dans les journaux d’audit</span><span class="sxs-lookup"><span data-stu-id="f40c4-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="f40c4-103">Vous pouvez utiliser la recherche de journal d’audit dans le centre de sécurité & conformité pour afficher les événements de règles de boîte de réception (création, modification et suppression de règles de boîte de réception).</span><span class="sxs-lookup"><span data-stu-id="f40c4-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="f40c4-104">Connectez-vous au [Centre de conformité & Office 365 Security](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f40c4-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="f40c4-105">Cliquez sur **recherche et enquête** , puis sélectionnez **recherche du journal d’audit**.</span><span class="sxs-lookup"><span data-stu-id="f40c4-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="f40c4-106">Sélectionnez la plage de dates dans les champs **Date de début** et **Date de fin** .</span><span class="sxs-lookup"><span data-stu-id="f40c4-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="f40c4-107">Sous **activités de boîte aux lettres Exchange**, vérifiez que le champ **activités** est défini sur **nouveau-InboxRule créer/modifier/activer/désactiver la règle de boîte de réception**.</span><span class="sxs-lookup"><span data-stu-id="f40c4-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="f40c4-108">Cliquez sur **Rechercher**.</span><span class="sxs-lookup"><span data-stu-id="f40c4-108">Click **Search**.</span></span>

<span data-ttu-id="f40c4-109">Dans les résultats, sélectionnez un enregistrement d’audit.</span><span class="sxs-lookup"><span data-stu-id="f40c4-109">In the results, select an audit record.</span></span> <span data-ttu-id="f40c4-110">Dans la fenêtre mobile des détails, cliquez sur **informations supplémentaires**.</span><span class="sxs-lookup"><span data-stu-id="f40c4-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f40c4-111">Les informations sur les paramètres des règles de boîte de réception sont affichées dans le champ **paramètres** .</span><span class="sxs-lookup"><span data-stu-id="f40c4-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="f40c4-112">Pour plus d’informations, consultez [la rubrique déterminer si un utilisateur a créé une règle de boîte de réception](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="f40c4-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
