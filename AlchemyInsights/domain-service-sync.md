---
title: Synchronisation du service de domaine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: 95b5c3b768caf4b5d80a088a17a33facb39805fc766e4888586ae052d91681e3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057856"
---
# <a name="domain-service-synchronization"></a>Synchronisation du service de domaine

Les objets et informations d’identification d’un domaine géré des services de domaine Azure Active Directory (Azure AD DS) peuvent être créés localement dans le domaine ou synchronisés à partir d’un client Azure Active Directory (Azure AD). Lorsque vous déployez Azure AD DS pour la première fois, une synchronisation à sens seul automatique est configurée et lancée pour répliquer les objets à partir d’Azure AD. Cette synchronisation à sens seul continue de s’exécuter en arrière-plan pour maintenir le domaine géré Azure AD DS à jour avec les modifications apportées à Azure AD. Aucune synchronisation n’a lieu à partir d’Azure AD DS vers Azure AD.

Pour plus d’informations sur Azure Active Directory de service de domaine, voir [Synchronisation des services de domaine.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 
