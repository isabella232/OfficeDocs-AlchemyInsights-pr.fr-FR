---
title: Un utilisateur ne voit pas de compléments dans Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154557"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="4536e-102">Un utilisateur ne voit pas de compléments dans Outlook</span><span class="sxs-lookup"><span data-stu-id="4536e-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="4536e-103">L’utilisateur peut faire partie d’un rôle qui ne présente pas le paramètre AppsForOfficeEnabled approprié.</span><span class="sxs-lookup"><span data-stu-id="4536e-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="4536e-104">Exécutez cette applet de commande pour déterminer si le rôle adéquat est associé à l’utilisateur :</span><span class="sxs-lookup"><span data-stu-id="4536e-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="4536e-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="4536e-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="4536e-106">Pour plus d'informations, voir [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="4536e-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
