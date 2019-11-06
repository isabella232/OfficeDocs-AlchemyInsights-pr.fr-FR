---
title: Rapports de journal d’audit SharePoint classiques
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992616"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f11df-102">Journaux d’audit SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="f11df-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f11df-103">Journaux d’audit SharePoint classiques</span><span class="sxs-lookup"><span data-stu-id="f11df-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f11df-104">SPO l’audit hérité a été migré vers le journal d’audit unifié.</span><span class="sxs-lookup"><span data-stu-id="f11df-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f11df-105">Tous les rapports d’audit hérités SPO seront désormais mis à l', et les signaux d’audit hérités ont été migrés vers le port.</span><span class="sxs-lookup"><span data-stu-id="f11df-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f11df-106">Modifications clés :</span><span class="sxs-lookup"><span data-stu-id="f11df-106">Key changes:</span></span>

* <span data-ttu-id="f11df-107">Le filtrage n’est pas disponible en tant que fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="f11df-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f11df-108">Le choix d’événements spécifiques à auditr n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="f11df-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f11df-109">Reportez-vous à [ce document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pour obtenir la liste complète des événements audités disponibles par défaut.</span><span class="sxs-lookup"><span data-stu-id="f11df-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f11df-110">L’option **emplacement** sous **rapports personnalisés** n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="f11df-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f11df-111">L’option d' **ouverture ou de téléchargement** des événements de documents n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="f11df-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f11df-112">Configurer les paramètres d’audit pour une collection de sites</span><span class="sxs-lookup"><span data-stu-id="f11df-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f11df-113">Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité</span><span class="sxs-lookup"><span data-stu-id="f11df-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f11df-114">Activer/désactiver la journalisation d’audit unifiée</span><span class="sxs-lookup"><span data-stu-id="f11df-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f11df-115">Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f11df-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f11df-116">Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :</span><span class="sxs-lookup"><span data-stu-id="f11df-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f11df-117">Activités de fichier et de page</span><span class="sxs-lookup"><span data-stu-id="f11df-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f11df-118">Activités de dossier</span><span class="sxs-lookup"><span data-stu-id="f11df-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f11df-119">Activités de partage et d’accès aux demandes</span><span class="sxs-lookup"><span data-stu-id="f11df-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f11df-120">Activités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="f11df-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f11df-121">Activités d’administration de site</span><span class="sxs-lookup"><span data-stu-id="f11df-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f11df-122">Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="f11df-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
