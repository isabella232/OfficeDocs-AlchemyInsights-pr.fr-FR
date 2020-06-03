---
title: Résoudre les problèmes de refus d’accès aux messages
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505377"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Résoudre les problèmes de refus d’accès aux messages dans le centre d’administration SharePoint/OneDrive

Si vous recevez un message de refus d’accès lorsque vous tentez d’accéder à un centre d’administration SharePoint/OneDrive, veillez [à attribuer une licence à l’utilisateur](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Si l’utilisateur dispose d’une licence, vous devez également vous assurer qu’il dispose [d’un rôle d’administrateur](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) pouvant accéder aux centres d’administration.

Ce problème peut également se produire lorsqu’un utilisateur est supprimé et recréé avec le nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une valeur PUID (ID unique Passport) différente. Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, l’utilisateur a un PUID incorrect. Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà connectés à SharePoint, puis sont déplacés vers une unité d’organisation différente et resynchronisés avec SharePoint, ils peuvent rencontrer ce problème.

Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes décrites dans l’article [restaurer un utilisateur dans Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Remarque : si un centre d’administration OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs ayant précédemment accès, il peut y avoir un problème de service temporaire.  [Vérifiez le tableau de bord d’État du service](https://portal.office.com/adminportal/home#/servicehealth).


