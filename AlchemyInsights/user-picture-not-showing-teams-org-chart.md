---
title: L'image de l'utilisateur ne s'affiche pas dans l'organigramme de Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467370"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>L'image de l'utilisateur ne s'affiche pas dans l'organigramme de Microsoft Teams

Si il manque les photos d’une ou plusieurs personnes de votre organisation dans l’organigramme, il est possible que le paramètre **ShowInAddressLists** soit définie sur **Non**:

1. Accédez au Centre d’administration Microsoft 365 > [**Utilisateurs actifs**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), puis sélectionnez l’utilisateur avec la photo manquante. 
1. Sélectionnez l’onglet **Courrier** et assurez-vous que l’onglet **Afficher dans la liste d’adresses globale** est définie sur **Oui**. 

Si la définition de **ShowInAddressLists** sur **Oui** ne fonctionne pas, vérifiez ce qui suit :

- L’utilisateur peut être masqué dans la liste des destinataires dans Exchange. Pour plus d’informations, consultez [Gérer les listes d’adresses Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- L’utilisateur peut être masqué dans la liste d’adresses Azure Active Directory. Pour plus d’informations, consultez [Définir un utilisateur Azure AD](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
