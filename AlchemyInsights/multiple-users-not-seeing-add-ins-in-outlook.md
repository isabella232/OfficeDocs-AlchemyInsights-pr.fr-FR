---
title: Plusieurs utilisateurs ne voient pas les compléments dans Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154561"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="3ac09-102">Plusieurs utilisateurs ne voient pas les compléments dans Outlook</span><span class="sxs-lookup"><span data-stu-id="3ac09-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="3ac09-103">Si vous testez les compléments Outlook et qu’aucun n’apparaît, commencez par utiliser l’applet de commande PowerShell **Get-OrganizationConfig** pour interroger le paramètre _AppsForOfficeEnabled_.</span><span class="sxs-lookup"><span data-stu-id="3ac09-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="3ac09-104">Si la requête renvoie la valeur **False**, définissez ce paramètre sur **True** à l’aide de l’applet de commande **OrganizationConfig**, de sorte que les compléments s’affichent comme prévu.</span><span class="sxs-lookup"><span data-stu-id="3ac09-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="3ac09-105">Nous vous déconseillons de définir le paramètre _AppsForOfficeEnabled_ sur **False**.</span><span class="sxs-lookup"><span data-stu-id="3ac09-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="3ac09-106">La valeur **False** remplace tous les paramètres de rôle d’administration et d’utilisateur ci-dessus, et empêche l’activation de nouvelles applications par les utilisateurs de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="3ac09-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="3ac09-107">Pour plus d'informations, consultez la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="3ac09-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>