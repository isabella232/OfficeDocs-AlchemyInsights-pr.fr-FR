---
title: Déploiement d’un GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067838"
---
# <a name="gpo-deployment"></a>Déploiement d’un GPO

Les paramètres des objets utilisateur et ordinateur dans Azure Active Directory Domain Services (Azure AD DS) sont souvent gérés à l’aide d’objets de stratégie de groupe. Azure AD DS inclut des objets de stratégie de groupe intégrés pour les utilisateurs AADDC et les conteneurs d’ordinateurs AADDC. Vous pouvez personnaliser ces objets de stratégie de groupe intégrés pour configurer une stratégie de groupe selon les besoins de votre environnement. Les membres du groupe d’administrateurs Azure AD DC ont des privilèges d’administration de stratégie de groupe dans le domaine Azure AD DS et peuvent également créer des objets de stratégies de groupe et des unités d’organisation personnalisées. Pour plus d’informations sur la stratégie de groupe et son fonctionnement, voir [Vue d’ensemble de la stratégie de groupe.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Dans un environnement hybride, les stratégies de groupe configurées dans un environnement AD DS local ne sont pas synchronisées avec Azure AD DS. Pour définir les paramètres de configuration des utilisateurs ou des ordinateurs dans Azure AD DS, modifiez l’un des objectifs de groupe par défaut ou créez un groupe de travail personnalisé.

Cet article [Gérer des stratégie de groupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) vous explique comment installer les outils de gestion des stratégies de groupe, comment modifier les objets de stratégie de groupe intégrés et comment créer des objets de stratégie de groupe personnalisés.
