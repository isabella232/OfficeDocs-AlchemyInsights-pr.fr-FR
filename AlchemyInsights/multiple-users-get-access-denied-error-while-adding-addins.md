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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="59eb9-102">L’erreur « Accès refusé » apparaît lorsque plusieurs utilisateurs ajoutent des compléments dans Outlook</span><span class="sxs-lookup"><span data-stu-id="59eb9-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="59eb9-p101">Vous pouvez spécifier les administrateurs de votre organisation qui disposent des autorisations pour installer et gérer les compléments Outlook. Vous pouvez également indiquer les utilisateurs au sein de votre organisation qui disposent des autorisations pour installer et gérer des compléments pour leur propre utilisation.</span><span class="sxs-lookup"><span data-stu-id="59eb9-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="59eb9-105">Si vous souhaitez en savoir plus, veuillez consulter la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="59eb9-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="59eb9-106">Pour vérifier que vous avez correctement attribué les autorisations d’un utilisateur, remplacez <Role Name> par le nom du rôle à vérifier, puis exécutez la commande suivante dans Exchange Online PowerShell :</span><span class="sxs-lookup"><span data-stu-id="59eb9-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="59eb9-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="59eb9-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="59eb9-108">Cet exemple vous montre comment vérifier à qui vous avez attribué des autorisations pour installer des compléments de l’Office Store pour l’organisation.</span><span class="sxs-lookup"><span data-stu-id="59eb9-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="59eb9-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="59eb9-109">PowerShell</span></span>

<span data-ttu-id="59eb9-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="59eb9-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="59eb9-111">Dans les résultats de Get-ManagementRoleAssignment, consultez les entrées de la colonne Utilisateurs effectifs.</span><span class="sxs-lookup"><span data-stu-id="59eb9-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="59eb9-112">Pour obtenir des informations détaillées sur la syntaxe et les paramètres, voir [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="59eb9-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 