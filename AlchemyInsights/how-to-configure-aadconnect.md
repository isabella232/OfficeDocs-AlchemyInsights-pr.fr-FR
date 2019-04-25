---
title: 646 comment configurer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399769"
---
# <a name="configure-sync-features"></a>Configurer les fonctionnalités de synchronisation

Azure AD Connect comprend plusieurs fonctionnalités qui sont activées par défaut ou que vous pouvez activer ultérieurement. Certaines fonctionnalités nécessitent une configuration supplémentaire dans des environnements spécifiques.

- Limites de [filtrage](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) les objets sont synchronisés avec Azure ad. Par défaut, tous les utilisateurs, contacts, groupes et comptes d'ordinateur Windows 10 sont synchronisés. Vous pouvez inclure ou exclure des objets en fonction de domaines, d'unités d'organisation ou d'autres attributs.

- La [synchronisation de hachage de mot de passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronise le hachage de mot de passe de l'Active Directory local vers Azure ad. Cela permet de gérer les mots de passe à un seul emplacement, mais d'utiliser le même mot de passe dans les environnements locaux et Cloud. Étant donné qu'Active Directory est la source faisant autorité, vous pouvez utiliser vos propres stratégies de mot de passe.

- [Self-service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permet aux utilisateurs de réinitialiser leur mot de passe dans le Cloud tout en continuant à appliquer votre stratégie de mot de passe locale.

- L' [écriture différée du périphérique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permet de réécrire les appareils enregistrés dans Azure ad dans l'annuaire Active Directory local afin qu'ils puissent être utilisés pour l'accès conditionnel.

- [Empêcher](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) les suppressions accidentelles est activée par défaut pour empêcher trop de suppressions d'objets simultanées (plus de 500 objets par synchronisation). Vous pouvez modifier ce paramètre pour répondre aux besoins de votre organisation.

- La [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) est activée par défaut pour les installations rapides et garantit la mise à jour permanente de votre version d'Azure ad Connect.
