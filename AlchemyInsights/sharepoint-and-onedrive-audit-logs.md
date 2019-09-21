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
# <a name="sharepoint-and-onedrive-audit-logs"></a>Journaux d’audit SharePoint et OneDrive

**Journaux d’audit unifiés SharePoint et OneDrive modernes à partir de la conformité**

- [Activer/désactiver la journalisation d’audit unifiée](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

Aucune configuration supplémentaire n’est requise dans SharePoint ou OneDrive.

- Utiliser la recherche dans la journalisation d’audit pour vérifier l’activité du (des) fichier (s), dossier (s), utilisateur (s), autorisations :

    - [Activités de fichier et de page](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [Activités de dossier](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [Activités de partage et d’accès aux demandes](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [Activités de synchronisation](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [Activités d’administration de site](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- Pour plus d’informations sur la récupération de ces événements, voir [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

**Journaux d’audit SharePoint classiques**

Nous avons migré l’audit hérité SPO vers le journal d’audit unifié. Cela signifie que tous les rapports d’audit hérités SPO seront désormais mis à l', et que les signaux d’audit hérités ont été migrés vers le port.

Modifications clés :

- Le rognage en tant que fonctionnalité n’est pas disponible.
- La section dans laquelle vous choisissez des événements spécifiques à auditr n’est pas disponible. Pour obtenir la liste complète des événements audités disponibles par défaut, reportez-vous à [ce document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .
- L’option « emplacement » sous **rapports personnalisés** n’est pas disponible. 
- Les événements « ouverture ou téléchargement de documents » ne sont pas disponibles. 

