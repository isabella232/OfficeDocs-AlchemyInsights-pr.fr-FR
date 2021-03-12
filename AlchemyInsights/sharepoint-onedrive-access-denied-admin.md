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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707952"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Résoudre les problèmes de messages d’accès refusé dans le Centre d’administration Sharepoint/OneDrive

Si vous recevez un message de refus d’accès lors de la tentative d’accès à un Centre d’administration Sharepoint/OneDrive, assurez-vous d’attribuer une licence [à l’utilisateur.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Si l’utilisateur dispose d’une licence, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) vous devez également vous assurer qu’un rôle d’administrateur lui est attribué et qu’il peut accéder aux centres d’administration.

Ce problème peut également se produire lorsqu’un utilisateur est supprimé et re-créé avec le même nom d’utilisateur principal (UPN). Le nouveau compte est créé à l’aide d’une autre valeur PUID (Passport Unique ID). Lorsque l’utilisateur tente d’accéder à une collection de sites ou à son OneDrive, il dispose d’un PUID incorrect. Un deuxième scénario implique la synchronisation d’annuaires avec une unité d’organisation Active Directory. Si les utilisateurs se sont déjà inscrits à SharePoint, puis sont déplacés vers une autre ouo et resyncés avec SharePoint, ils peuvent être face à ce problème.

Pour résoudre ce problème, vous devez restaurer l’UPN d’origine en suivant les étapes de l’article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Remarque : si un centre d’administration OneDrive ou SharePoint n’est pas disponible pour plusieurs utilisateurs qui y avaient précédemment accès, il peut y avoir un problème de service temporaire.  [Vérifiez le tableau de bord d’état du service.](https://portal.office.com/adminportal/home#/servicehealth)


