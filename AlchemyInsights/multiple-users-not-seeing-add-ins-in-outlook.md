---
title: Plusieurs utilisateurs ne voient pas les compléments dans Outlook
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729869"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Plusieurs utilisateurs ne voient pas les compléments dans Outlook

Si vous testez les compléments Outlook et qu’aucun n’apparaît, commencez par utiliser l’applet de commande PowerShell **Get-OrganizationConfig** pour interroger le paramètre _AppsForOfficeEnabled_. Si la requête renvoie la valeur **False**, définissez ce paramètre sur **True** à l’aide de l’applet de commande **OrganizationConfig**, de sorte que les compléments s’affichent comme prévu.

Nous vous déconseillons de définir le paramètre _AppsForOfficeEnabled_ sur **False**. La valeur **False** remplace tous les paramètres de rôle d’administration et d’utilisateur ci-dessus, et empêche l’activation de nouvelles applications par les utilisateurs de l’organisation.

Pour plus d'informations, consultez la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).