---
title: L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724361"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook

Vous pouvez spécifier les administrateurs de votre organisation qui disposent des autorisations pour installer et gérer les compléments Outlook. Vous pouvez également indiquer les utilisateurs au sein de votre organisation qui disposent des autorisations pour installer et gérer des compléments pour leur propre utilisation.

Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Pour vérifier que vous avez correctement attribué les autorisations d’un utilisateur, remplacez <Role Name> par le nom du rôle à vérifier, puis exécutez la commande suivante dans Exchange Online PowerShell :

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

Cet exemple vous montre comment vérifier à qui vous avez attribué des autorisations pour installer des compléments de l’Office Store pour l’organisation.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Dans les résultats de Get-ManagementRoleAssignment, consultez les entrées de la colonne Utilisateurs effectifs.

Pour obtenir des informations détaillées sur la syntaxe et les paramètres, voir [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 