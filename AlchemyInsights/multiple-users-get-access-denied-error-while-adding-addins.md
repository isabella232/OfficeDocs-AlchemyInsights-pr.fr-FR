---
title: L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397717"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook

Vous pouvez spécifier les administrateurs de votre organisation qui disposent des autorisations pour installer et gérer les compléments Outlook. Vous pouvez également indiquer les utilisateurs au sein de votre organisation qui disposent des autorisations pour installer et gérer des compléments pour leur propre utilisation.

Pour plus d'informations, consultez la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Pour vérifier que vous avez correctement attribué les autorisations d’un utilisateur, remplacez <Role Name> par le nom du rôle à vérifier, puis exécutez la commande suivante dans Exchange Online PowerShell :

Get-ManagementRoleAssignment -Role « <Role Name> » -GetEffectiveUsers

Cet exemple vous montre comment vérifier à qui vous avez attribué des autorisations pour installer des compléments de l’Office Store pour l’organisation.

PowerShell

-Role « Applications Marketplace d’organisation » : GetEffectiveUsers

Dans les résultats, Get-ManagementRoleAssignment, consultez les entrées de la colonne Utilisateurs effectifs.

Pour obtenir des informations détaillées sur la syntaxe et les paramètres, voir [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 