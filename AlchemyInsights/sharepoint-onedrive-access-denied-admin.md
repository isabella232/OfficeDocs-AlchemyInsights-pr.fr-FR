---
title: Résoudre les problèmes de messages d’accès refusé
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085226"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Résoudre les problèmes de messages d’accès refusé dans le Centre d’administration Sharepoint/OneDrive

Si vous recevez un message de refus d’accès lors de la tentative d’accès à un Centre d’administration Sharepoint/OneDrive, assurez-vous d’attribuer une licence à [l’utilisateur.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Si l’utilisateur dispose d’une licence, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) vous devez également vous assurer qu’un rôle d’administrateur lui est attribué et qu’il peut accéder aux centres d’administration.

Ce problème peut également se produire lorsqu’un utilisateur est supprimé et re-créé avec le même nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une valeur PUID (Passport Unique ID) différente. Lorsque l’utilisateur tente d’accéder à une collection de sites ou à sa OneDrive, il dispose d’un PUID incorrect. Un second scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà SharePoint, puis sont déplacés vers une autre ouo et resyncés avec SharePoint, ils peuvent être face à ce problème.

Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes de l’article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Remarque : si un centre d’administration OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui y avaient précédemment accès, il se peut qu’il y a un problème de service temporaire.  [Vérifiez le tableau de bord d’état du service.](https://portal.office.com/adminportal/home#/servicehealth)


