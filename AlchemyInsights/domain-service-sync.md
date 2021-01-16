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
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876515"
---
# <a name="domain-service-synchronization"></a>Synchronisation du service de domaine

Les objets et informations d’identification d’un domaine géré Azure Active Directory Domain Services (Azure AD DS) peuvent être créés localement dans le domaine ou synchronisés à partir d’un client Azure Active Directory (Azure AD). Lorsque vous déployez Azure AD DS pour la première fois, une synchronisation à sens seul automatique est configurée et lancée pour répliquer les objets à partir d’Azure AD. Cette synchronisation à sens seul continue de s’exécuter en arrière-plan pour maintenir le domaine géré Azure AD DS à jour avec les modifications apportées à Azure AD. Aucune synchronisation n’a lieu à partir d’Azure AD DS vers Azure AD.

Pour plus d’informations sur la synchronisation du service de domaine Azure Active Directory, voir [Synchronisation des services de domaine.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization) 
