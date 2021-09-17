---
title: La photo de l'utilisateur apparaît toujours dans l'organigramme de Microsoft Teams.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334363"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>La photo de l'utilisateur apparaît toujours dans l'organigramme de Microsoft Teams.

Si une ou plusieurs personnes de votre organisation ont été désactivées ou supprimées, et que leur photo de profil apparaît toujours dans l'organigramme, il est possible que le paramètre **ShowInAddressLists** soit réglé sur False : 

1. Allez dans le centre d'administration Microsoft 365 > [Utilisateurs actifs](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) et sélectionnez l'utilisateur dont la photo apparaît toujours. 
1. Sélectionnez **l’onglet** Courrier et assurez-vous que **l’onglet** Afficher dans la liste d’adresses globale est définie sur **Non**.

Si la définition **de ShowInAddressLists** sur **Non** ne fonctionne pas, vérifiez ce qui suit : 

- L’utilisateur peut être affiché dans la liste des destinataires dans Exchange. Pour plus d’informations, consultez [Gérer les listes d’adresses Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- L’utilisateur peut être affiché dans la liste d’adresses Azure Active Directory. Pour plus d’informations, consultez [Définir un utilisateur Azure AD](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 