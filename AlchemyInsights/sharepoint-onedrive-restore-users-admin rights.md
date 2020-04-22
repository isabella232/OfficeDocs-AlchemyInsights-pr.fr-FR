---
title: Dépannage des messages refusés d’accès aux sites OneDrive entreprise
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692799"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Dépannage des messages refusés d’accès aux sites OneDrive entreprise

Ce problème se produit le plus souvent lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente. Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect. Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.

1. Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article [restaurer un utilisateur dans Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. Si vous ne pouvez pas restaurer l’utilisateur d’origine, vous devez supprimer l’ancien utilisateur du site OneDrive en suivant ces étapes, [supprimer un utilisateur de la liste d’informations utilisateur](). 
3. Une fois cette opération terminée, vous pouvez vérifier que l’utilisateur dispose de droits d’administrateur sur le site OneDrive en suivant les étapes d’ajout de l' [administrateur pour le onedrive d’un utilisateur](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Pour plus d’informations sur les niveaux d’autorisation, voir l’article relatif aux [niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
