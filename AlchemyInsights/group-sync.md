---
title: Synchronisation des groupes
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
- "8304"
- "9003234"
ms.openlocfilehash: 7e5ed69c34f8e7b922d7eef202af508152a7e04d7773581b32e43395571c6fbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987645"
---
# <a name="group-sync"></a>Synchronisation des groupes

Cet article fournit des conseils sur la synchronisation des groupes.

1. Si un administrateur général ou propriétaire de groupe n’est pas en mesure de modifier les propriétés du groupe ou d’ajouter des membres ou d’attribuer des propriétaires dans le Portail Microsoft Azure, assurez-vous que la source de l’autorité pour le groupe est Azure Active Directory (Azure AD) pour l’administrateur général ou le propriétaire du groupe afin de modifier le groupe.
2. Avant d’essayer de supprimer un groupe synchronisé dans Azure AD, assurez-vous que vous avez [supprimé toutes les licences attribuées](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) pour éviter les erreurs.

Pour comprendre comment synchroniser les utilisateurs, les groupes et les contacts, consultez [Synchronisation d’Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), et suivez [Synchronisation d’un groupe local sur Azure à l’aide d’Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) pour synchroniser des groupes locaux à l’aide de Azure AD Connect.

Suivez ce guide [Erreurs de résolution des problèmes pendant la synchronisation](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) pour résoudre des problèmes d’erreurs courantes lors de la synchronisation.

