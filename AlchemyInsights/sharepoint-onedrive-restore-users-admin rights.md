---
title: Résolution des problèmes d’accès aux messages refusés OneDrive Entreprise sites
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957791"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Résolution des problèmes d’accès aux messages refusés OneDrive Entreprise sites

Ce problème se produit le plus souvent lorsqu’un utilisateur est supprimé et re-créé avec le même nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une valeur PUID (Passport Unique ID) différente. Lorsque l’utilisateur tente d’accéder à une collection de sites ou à sa OneDrive, il dispose d’un PUID incorrect. Un second scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà SharePoint, puis sont déplacés vers une autre ouo et resyncés avec SharePoint, ils peuvent être face à ce problème.

1. Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes de l’article, restituer un utilisateur [dans Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Si vous ne pouvez pas restaurer l’utilisateur d’origine, vous devez supprimer l’ancien utilisateur du site OneDrive à l’aide de ces étapes, supprimez un utilisateur de la [liste d’informations utilisateur.]() 
3. Une fois cette étape effectuée, vous pouvez vérifier que l’utilisateur dispose des droits d’administrateur sur le site OneDrive en suivant les étapes pour ajouter des administrateurs pour le compte [d’un OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Pour plus d’informations sur les niveaux d’autorisation, consultez l’article « [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels)».
