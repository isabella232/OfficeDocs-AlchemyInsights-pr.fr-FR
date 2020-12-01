---
title: Supprimer un locataire
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477677"
---
# <a name="delete-tenant"></a>Supprimer un locataire

Pour supprimer un Azure AD, vérifiez les éléments suivants :
- Vous êtes un administrateur général de l’annuaire.
- Vous n’êtes pas connecté avec un compte qui a le répertoire par défaut tel que contoso.onmicrosoft.com dans le compte connecté, tel que admin@contoso.onmicrosoft.com.
- Supprimez toutes les applications actives dans l’annuaire avant la suppression. Pour supprimer des applications actives, accédez à inscriptions des applications et supprimez les applications existantes.
- Il n’existe aucun abonnement actif pour Microsoft Online Services, tel que Microsoft Azure, Office 365 ou Azure AD Premium associé à l’annuaire. Transférez vos abonnements ou Accélérez l’annulation des abonnements actifs via la prise en charge et la facturation Azure. Pour en savoir plus, consultez la procédure d’annulation des abonnements Office 365 et Azure. Pour obtenir des instructions sur l’Association ou l’ajout d’un abonnement existant à un client, reportez-vous à [la rubrique associer ou ajouter un abonnement Azure à votre client Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Il n’y a pas de licence active. Pour supprimer des licences, consultez [la rubrique How to Remove Subscription to Remove License](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Il n’y a pas d’autres utilisateurs actifs dans l’annuaire, outre vous-même en tant qu’administrateur général lors de la tentative de suppression d’Azure AD. Supprimez tous les autres utilisateurs actifs, et toutes les dépendances d’un nom de domaine personnalisé dans le client doivent également être supprimées, telles que les utilisateurs créés avec admin@contoso.com.

Pour plus d’informations sur la procédure :
- Supprimez « Azure Active Directory » ou « abonnement », consultez la rubrique [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Suppression d’applications dans l’annuaire, consultez la rubrique [Suppression d’applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
