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
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509598"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Journaux d’audit SharePoint et OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Journaux d’audit SharePoint classiques

SPO l’audit hérité a été migré vers le journal d’audit unifié. Tous les rapports d’audit hérités SPO seront désormais mis à l', et les signaux d’audit hérités ont été migrés vers le port.

Modifications clés :

* Le filtrage n’est pas disponible en tant que fonctionnalité.
* Le choix d’événements spécifiques à auditr n’est pas disponible. Reportez-vous à [ce document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) pour obtenir la liste complète des événements audités disponibles par défaut.
* L’option **emplacement** sous **rapports personnalisés** n’est pas disponible.
* L’option d' **ouverture ou de téléchargement** des événements de documents n’est pas disponible.

[Configurer les paramètres d’audit pour une collection de sites](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité

* [Activer/désactiver la journalisation d’audit unifiée](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.

Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :

* [Activités des fichiers et pages](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Activités des dossiers](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Activités de demande d’accès et de partage](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Activités de synchronisation](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Activités d’administration des sites](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
