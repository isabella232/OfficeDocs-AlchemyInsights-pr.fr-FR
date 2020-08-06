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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="e8705-102">L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook</span><span class="sxs-lookup"><span data-stu-id="e8705-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="e8705-p101">Vous pouvez spécifier les administrateurs de votre organisation qui disposent des autorisations pour installer et gérer les compléments Outlook. Vous pouvez également indiquer les utilisateurs au sein de votre organisation qui disposent des autorisations pour installer et gérer des compléments pour leur propre utilisation.</span><span class="sxs-lookup"><span data-stu-id="e8705-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="e8705-105">Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e8705-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="e8705-106">Pour vérifier que vous avez correctement attribué les autorisations d’un utilisateur, remplacez <Role Name> par le nom du rôle à vérifier, puis exécutez la commande suivante dans Exchange Online PowerShell :</span><span class="sxs-lookup"><span data-stu-id="e8705-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e8705-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e8705-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="e8705-108">Cet exemple vous montre comment vérifier à qui vous avez attribué des autorisations pour installer des compléments de l’Office Store pour l’organisation.</span><span class="sxs-lookup"><span data-stu-id="e8705-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="e8705-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="e8705-109">PowerShell</span></span>

<span data-ttu-id="e8705-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e8705-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="e8705-111">Dans les résultats de Get-ManagementRoleAssignment, consultez les entrées de la colonne Utilisateurs effectifs.</span><span class="sxs-lookup"><span data-stu-id="e8705-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="e8705-112">Pour obtenir des informations détaillées sur la syntaxe et les paramètres, voir [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="e8705-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 