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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068021"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="fe262-102">Journaux d’audit SharePoint et OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe262-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="fe262-103">**Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité**</span><span class="sxs-lookup"><span data-stu-id="fe262-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="fe262-104">Activer/désactiver la journalisation d’audit unifiée</span><span class="sxs-lookup"><span data-stu-id="fe262-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="fe262-105">Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fe262-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="fe262-106">Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :</span><span class="sxs-lookup"><span data-stu-id="fe262-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="fe262-107">Activités de fichier et de page</span><span class="sxs-lookup"><span data-stu-id="fe262-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="fe262-108">Activités de dossier</span><span class="sxs-lookup"><span data-stu-id="fe262-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="fe262-109">Activités de partage et d’accès aux demandes</span><span class="sxs-lookup"><span data-stu-id="fe262-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="fe262-110">Activités de synchronisation</span><span class="sxs-lookup"><span data-stu-id="fe262-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="fe262-111">Activités d’administration de site</span><span class="sxs-lookup"><span data-stu-id="fe262-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="fe262-112">Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="fe262-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="fe262-113">**Journaux d’audit SharePoint classiques**</span><span class="sxs-lookup"><span data-stu-id="fe262-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="fe262-114">Nous avons migré l’audit hérité SPO vers le journal d’audit unifié.</span><span class="sxs-lookup"><span data-stu-id="fe262-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="fe262-115">Cela signifie que tous les rapports d’audit hérités SPO seront désormais mis à l', et que les signaux d’audit hérités ont été migrés vers le port.</span><span class="sxs-lookup"><span data-stu-id="fe262-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="fe262-116">Modifications clés :</span><span class="sxs-lookup"><span data-stu-id="fe262-116">Key changes:</span></span>

- <span data-ttu-id="fe262-117">Le rognage en tant que fonctionnalité n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="fe262-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="fe262-118">La section dans laquelle vous choisissez des événements spécifiques à auditr n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="fe262-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="fe262-119">Pour obtenir la liste complète des événements audités disponibles par défaut, reportez-vous à [ce document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .</span><span class="sxs-lookup"><span data-stu-id="fe262-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="fe262-120">L’option « emplacement » sous **rapports personnalisés** n’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="fe262-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="fe262-121">Les événements « ouverture ou téléchargement de documents » ne sont pas disponibles.</span><span class="sxs-lookup"><span data-stu-id="fe262-121">“Opening or downloading documents” events is NOT available.</span></span> 

