---
title: Stratégie de groupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: 5bccaedda08e2c948a15c0b32c6f6eeecfc8bd4c4555b25291f294fe5deb3019
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088790"
---
# <a name="group-policy"></a>Stratégie de groupe

Les paramètres des objets utilisateur et ordinateur dans Azure Active Directory Domain Services (Azure AD DS) sont souvent gérés à l’aide d’objets de stratégie de groupe. Azure AD DS inclut des objets de stratégie de groupe intégrés pour les utilisateurs AADDC et les conteneurs d’ordinateurs AADDC. Vous pouvez personnaliser ces objets de stratégie de groupe intégrés pour configurer une stratégie de groupe selon les besoins de votre environnement. Les membres du groupe d’administrateurs Azure AD DC ont des privilèges d’administration de stratégie de groupe dans le domaine Azure AD DS et peuvent également créer des objets de stratégies de groupe et des unités d’organisation personnalisées. Pour plus d’informations sur la stratégie de groupe et son fonctionnement, consultez [Vue d’ensemble des stratégies de groupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Dans un environnement hybride, les stratégies de groupe configurées dans un environnement AD DS local ne sont pas synchronisées avec Azure AD DS. Pour définir les paramètres de configuration des utilisateurs ou des ordinateurs dans Azure AD DS, modifiez l’un des objectifs de groupe par défaut ou créez un groupe de travail personnalisé.

Cet article [Gérer des stratégie de groupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vous explique comment installer les outils de gestion des stratégies de groupe, comment modifier les objets de stratégie de groupe intégrés et comment créer des objets de stratégie de groupe personnalisés.



