---
title: Rapports de journal d’audit SharePoint classiques
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741963"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="4d63c-102">Journaux d’audit SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="4d63c-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="4d63c-103">Journaux d’audit SharePoint classiques</span><span class="sxs-lookup"><span data-stu-id="4d63c-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="4d63c-104">SPO l’audit hérité a été migré vers le journal d’audit unifié.</span><span class="sxs-lookup"><span data-stu-id="4d63c-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="4d63c-105">Tous les rapports d’audit hérités SPO seront désormais mis à l', et les signaux d’audit hérités ont été migrés vers le port.</span><span class="sxs-lookup"><span data-stu-id="4d63c-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="4d63c-106">Modifications clés :</span><span class="sxs-lookup"><span data-stu-id="4d63c-106">Key changes:</span></span>

* <span data-ttu-id="4d63c-107">Le filtrage n’est pas disponible en tant que fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="4d63c-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="4d63c-108">Le choix d’événements spécifiques à auditr n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="4d63c-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="4d63c-109">Reportez-vous à [ce document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) pour obtenir la liste complète des événements audités disponibles par défaut.</span><span class="sxs-lookup"><span data-stu-id="4d63c-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="4d63c-110">L’option **emplacement** sous **rapports personnalisés** n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="4d63c-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="4d63c-111">L’option d' **ouverture ou de téléchargement** des événements de documents n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="4d63c-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="4d63c-112">Configurer les paramètres d’audit pour une collection de sites</span><span class="sxs-lookup"><span data-stu-id="4d63c-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="4d63c-113">Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité</span><span class="sxs-lookup"><span data-stu-id="4d63c-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="4d63c-114">Activer/désactiver la journalisation d’audit unifiée</span><span class="sxs-lookup"><span data-stu-id="4d63c-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="4d63c-115">Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4d63c-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="4d63c-116">Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :</span><span class="sxs-lookup"><span data-stu-id="4d63c-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="4d63c-117">Activités des fichiers et pages</span><span class="sxs-lookup"><span data-stu-id="4d63c-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="4d63c-118">Activités des dossiers</span><span class="sxs-lookup"><span data-stu-id="4d63c-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="4d63c-119">Activités de demande d’accès et de partage</span><span class="sxs-lookup"><span data-stu-id="4d63c-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="4d63c-120">Activités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="4d63c-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="4d63c-121">Activités d’administration des sites</span><span class="sxs-lookup"><span data-stu-id="4d63c-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="4d63c-122">Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="4d63c-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
