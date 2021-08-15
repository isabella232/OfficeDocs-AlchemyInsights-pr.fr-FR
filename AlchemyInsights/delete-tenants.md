---
title: Supprimer un client
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993891"
---
# <a name="delete-tenant"></a>Supprimer un client

Pour supprimer un Azure AD, assurez-vous que :
- Vous êtes administrateur général sur l’annuaire.
- Vous n’êtes PAS signé avec un compte qui possède le répertoire par défaut tel que contoso.onmicrosoft.com dans le compte de la admin@contoso.onmicrosoft.com.
- Supprimez toutes les applications actives dans le répertoire avant la suppression. Pour supprimer des applications actives, accédez aux inscriptions d’applications et supprimez les applications existantes.
- Aucun abonnement actif n’est Microsoft Online Services, tel que Microsoft Azure, Office 365 ou Azure AD Premium sur l’annuaire. Transférez vos abonnements ou accélèrez l’annulation des abonnements actifs via le support et la facturation Azure. En savoir plus sur la façon d’annuler Office 365 abonnements Azure. Pour obtenir des instructions sur l’association ou l’ajout d’un abonnement existant à un client, voir Associer ou ajouter un abonnement Azure à votre client [Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Il n’existe aucune licence active. Pour supprimer des licences, voir [Comment supprimer l’abonnement pour supprimer une licence](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Il n’y a pas d’autres utilisateurs actifs dans l’annuaire que vous en tant qu’administrateur général lors de la tentative de suppression d’Azure AD. Supprimez tous les autres utilisateurs actifs et les dépendances sur un nom de domaine personnalisé dans le client devront également être supprimées, telles que les utilisateurs créés avec admin@contoso.com.

Pour plus d’informations sur la procédure à suivre :
- Supprimez « Azure Active Directory » ou « abonnement », voir [Supprimer Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Suppression d’applications dans le répertoire, voir [Suppression d’applications.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
