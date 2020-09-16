---
title: Problèmes liés à l’utilisation de la console d’administration Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728285"
---
# <a name="problems-using-the-intune-admin-console"></a>Problèmes liés à l’utilisation de la console d’administration Intune

**« Accès refusé » lors de la navigation dans le portail d’administration Intune.**

- Si vous êtes membre d’un rôle personnalisé Intune, vérifiez qu’une licence Intune ou Enterprise Mobility Suite (EMS) est attribuée à votre compte.
- Si vous utilisez Configuration Manager pour gérer les appareils, vérifiez que vous ne faites pas partie de la collection d’utilisateurs Intune pour Configuration Manager MDM.
- Vérifiez que les autorisations de contrôle d’administration basée sur les rôles (RBAC) appropriées vous sont attribuées dans le panneau de rôles Intune.
- Vérifiez que le groupe utilisé n’est pas une liste de distribution. Intune dans le portail Microsoft Azure prend uniquement en charge les comptes d’utilisateur appartenant aux groupes de sécurité Azure Active Directory. Vérifiez vos groupes sur le portail Microsoft Azure > **Intune** > **Groupes**, ou sur le portail Microsoft Azure > **Azure Active Directory**.

**L’utilisateur a trop d’autorisations pour le rôle Intune attribué**

Invitez l’utilisateur à accéder à **Intune** > **Rôles Intune** > **Mes autorisations** > **Exporter** pour vérifier les autorisations accordées.

**J’ai ajouté un groupe d’étendues à un rôle, mais les utilisateurs de ce rôle voient toujours les autres utilisateurs ou appareils.**

Les groupes d’étendues ne filtrent pas les utilisateurs ou les appareils. Groupes d’étendues :

- Limiter les utilisateurs auxquels vous pouvez attribuer les stratégies ou applications.
- Autoriser uniquement des utilisateurs spécifiques à exécuter des tâches distantes sur des appareils.

Si vous souhaitez obtenir davantage d’informations sur les groupes d’étendues, voir [Contrôle d’accès en fonction du rôle (RBAC) avec Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**J’ai ajouté un utilisateur à un rôle Intune, mais il dispose toujours d’un accès complet à la console d’administration Intune.**

Accédez à Intune > **Utilisateurs** sur le portail Microsoft Azure et vérifiez que l’un des rôles suivants n’est pas attribué à l’utilisateur sur le portail Microsoft Azure :

- Administrateur général
- Administrateur du service Intune
- Administrateur SharePoint

Si vous souhaitez obtenir plus d’informations, consultez la page [Contrôle d’accès en fonction du rôle (RBAC) avec Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problèmes d’accès**

Si vous souhaitez obtenir davantage d’informations, consultez la page [Vous ne pouvez pas vous connecter à Office 365, Azure ou Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).