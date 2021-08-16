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
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011802"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Plusieurs utilisateurs ne voient pas les compléments dans Outlook

Si vous testez les compléments Outlook et qu’aucun n’apparaît, commencez par utiliser l’applet de commande PowerShell **Get-OrganizationConfig** pour interroger le paramètre _AppsForOfficeEnabled_. Si la requête renvoie la valeur **False**, définissez ce paramètre sur **True** à l’aide de l’applet de commande **OrganizationConfig**, de sorte que les compléments s’affichent comme prévu.

Nous ne recommandons pas que le paramètre _AppsForOfficeEnabled_ soit défini sur **False**. Une valeur **False** annule tous les paramètres des rôles d'administrateur et d'utilisateur ci-dessus et empêche l'activation de toute nouvelle application par tout utilisateur de l'organisation.

Pour plus d'informations, consultez la rubrique [Désigner les administrateurs et utilisateurs qui peuvent installer et gérer des compléments pour Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).