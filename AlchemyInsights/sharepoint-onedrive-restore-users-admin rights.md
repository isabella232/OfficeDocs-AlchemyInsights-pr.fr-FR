---
title: Donner aux utilisateurs l’accès à SharePoint et OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9326932e93970edc96396a141c9b36b14e7b4d4d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736646"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Donner aux utilisateurs l’accès à SharePoint et OneDrive

Ce problème se produit le plus souvent lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente. Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect. Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.

Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article[restaurer un utilisateur dans Office 365](https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide).

Une fois cette opération terminée, vous pouvez vérifier que l’utilisateur dispose de droits d’administrateur sur le site OneDrive en suivant les étapes d’ajout de l' [administrateur pour le onedrive d’un utilisateur](https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive) .

Pour plus d’informations sur les niveaux d’autorisation, voir l’article relatif aux [niveaux d’autorisation dans SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
