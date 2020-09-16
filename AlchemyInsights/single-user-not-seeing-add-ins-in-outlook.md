---
title: Un utilisateur ne voit pas de compléments dans Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719663"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Un utilisateur ne voit pas de compléments dans Outlook

L’utilisateur peut faire partie d’un rôle qui ne présente pas le paramètre AppsForOfficeEnabled approprié. Exécutez cette applet de commande pour déterminer si le rôle adéquat est associé à l’utilisateur :

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Pour plus d'informations, voir [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
