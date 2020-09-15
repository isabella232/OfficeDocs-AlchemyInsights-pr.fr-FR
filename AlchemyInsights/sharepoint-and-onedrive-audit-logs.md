---
title: Rapports de journal d’audit SharePoint classiques
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662206"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="5b58b-102">Journaux d’audit SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="5b58b-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="5b58b-103">Journaux d’audit SharePoint classiques</span><span class="sxs-lookup"><span data-stu-id="5b58b-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="5b58b-104">SPO l’audit hérité a été migré vers le journal d’audit unifié.</span><span class="sxs-lookup"><span data-stu-id="5b58b-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="5b58b-105">Tous les rapports d’audit hérités SPO seront désormais mis à l', et les signaux d’audit hérités ont été migrés vers le port.</span><span class="sxs-lookup"><span data-stu-id="5b58b-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="5b58b-106">Modifications clés :</span><span class="sxs-lookup"><span data-stu-id="5b58b-106">Key changes:</span></span>

* <span data-ttu-id="5b58b-107">Le filtrage n’est pas disponible en tant que fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="5b58b-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="5b58b-108">Le choix d’événements spécifiques à auditr n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="5b58b-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="5b58b-109">Reportez-vous à [ce document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) pour obtenir la liste complète des événements audités disponibles par défaut.</span><span class="sxs-lookup"><span data-stu-id="5b58b-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="5b58b-110">L’option **emplacement** sous **rapports personnalisés** n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="5b58b-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="5b58b-111">L’option d' **ouverture ou de téléchargement** des événements de documents n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="5b58b-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="5b58b-112">Configurer les paramètres d’audit pour une collection de sites</span><span class="sxs-lookup"><span data-stu-id="5b58b-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="5b58b-113">Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité</span><span class="sxs-lookup"><span data-stu-id="5b58b-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="5b58b-114">Activer/désactiver la journalisation d’audit unifiée</span><span class="sxs-lookup"><span data-stu-id="5b58b-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="5b58b-115">Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5b58b-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="5b58b-116">Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :</span><span class="sxs-lookup"><span data-stu-id="5b58b-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="5b58b-117">Activités des fichiers et pages</span><span class="sxs-lookup"><span data-stu-id="5b58b-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="5b58b-118">Activités des dossiers</span><span class="sxs-lookup"><span data-stu-id="5b58b-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="5b58b-119">Activités de demande d’accès et de partage</span><span class="sxs-lookup"><span data-stu-id="5b58b-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="5b58b-120">Activités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="5b58b-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="5b58b-121">Activités d’administration des sites</span><span class="sxs-lookup"><span data-stu-id="5b58b-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="5b58b-122">Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="5b58b-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
