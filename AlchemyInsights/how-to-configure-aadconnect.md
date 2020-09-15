---
title: 646 comment configurer AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704487"
---
# <a name="configure-sync-features"></a>Configurer les fonctionnalités de synchronisation

Azure AD Connect comprend plusieurs fonctionnalités qui sont activées par défaut ou que vous pouvez activer ultérieurement. Certaines fonctionnalités nécessitent une configuration supplémentaire dans des environnements spécifiques.

- Limites de [filtrage](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) les objets sont synchronisés avec Azure ad. Par défaut, tous les utilisateurs, contacts, groupes et comptes d’ordinateur Windows 10 sont synchronisés. Vous pouvez inclure ou exclure des objets en fonction de domaines, d’unités d’organisation ou d’autres attributs.

- La [synchronisation de hachage de mot de passe](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronise le hachage de mot de passe de l’Active Directory local vers Azure ad. Cela permet de gérer les mots de passe à un seul emplacement, mais d’utiliser le même mot de passe dans les environnements locaux et Cloud. Étant donné qu’Active Directory est la source faisant autorité, vous pouvez utiliser vos propres stratégies de mot de passe.

- [Self-service Password Reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permet aux utilisateurs de réinitialiser leur mot de passe dans le Cloud tout en continuant à appliquer votre stratégie de mot de passe locale.

- L' [écriture différée du périphérique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) permet de réécrire les appareils enregistrés dans Azure ad dans l’annuaire Active Directory local afin qu’ils puissent être utilisés pour l’accès conditionnel.

- [Empêcher les suppressions accidentelles](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) est activée par défaut pour empêcher trop de suppressions d’objets simultanées (plus de 500 objets par synchronisation). Vous pouvez modifier ce paramètre pour répondre aux besoins de votre organisation.

- La [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) est activée par défaut pour les installations rapides et garantit la mise à jour permanente de votre version d’Azure ad Connect.
