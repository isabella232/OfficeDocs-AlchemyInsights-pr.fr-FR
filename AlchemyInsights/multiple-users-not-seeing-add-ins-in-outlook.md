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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Plusieurs utilisateurs ne voient pas les compléments dans Outlook

Si vous testez les compléments Outlook et qu’aucun n’apparaît, commencez par utiliser l’applet de commande PowerShell **Get-OrganizationConfig** pour interroger le paramètre _AppsForOfficeEnabled_. Si la requête renvoie la valeur **False**, définissez ce paramètre sur **True** à l’aide de l’applet de commande **OrganizationConfig**, de sorte que les compléments s’affichent comme prévu.

Nous vous déconseillons de définir le paramètre _AppsForOfficeEnabled_ sur **False**. La valeur **False** remplace tous les paramètres de rôle d’administration et d’utilisateur ci-dessus, et empêche l’activation de nouvelles applications par les utilisateurs de l’organisation.

Pour plus d'informations, consultez la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).