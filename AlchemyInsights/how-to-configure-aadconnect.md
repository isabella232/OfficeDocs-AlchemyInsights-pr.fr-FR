---
title: 646 Comment configurer AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963641"
---
# <a name="configure-sync-features"></a>Configurer les fonctionnalités de synchronisation

Azure AD Connecter comprend plusieurs fonctionnalités activées par défaut, ou que vous pouvez activer ultérieurement. Certaines fonctionnalités nécessitent une configuration supplémentaire dans des environnements spécifiques.

- [Le filtrage](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limite la synchronisation des objets avec Azure AD. Par défaut, tous les utilisateurs, contacts, groupes Windows 10 comptes d’ordinateur sont synchronisés. Vous pouvez inclure ou exclure des objets basés sur des domaines, des objets d’entreprise ou d’autres attributs.

- [La synchronisation de hachage de](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) mot de passe synchronise le hachage de mot de passe à partir d’Active Directory local avec Azure AD. Cela permet la gestion des mots de passe à un seul emplacement, mais l’utilisation du même mot de passe dans les environnements locaux et cloud. Active Directory étant la source faisant autorité, vous pouvez utiliser vos propres stratégies de mot de passe.

- La réinitialisation du mot de passe en [libre-service (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) permet aux utilisateurs de réinitialiser leurs propres mots de passe dans le cloud tout en appliquant votre stratégie de mot de passe sur site.

- [L’écriture écriture sur](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) appareil permet aux appareils inscrits dans Azure AD d’être enregistrés dans l’annuaire Active Directory local afin qu’ils soient utilisés pour l’accès conditionnel.

- [La prévention des suppressions accidentelles](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) est activée par défaut pour éviter un trop grand nombre de suppressions simultanées d’objets (plus de 500 objets par synchronisation). Vous pouvez modifier ce paramètre pour répondre aux besoins de votre organisation.

- [La mise à](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) niveau automatique est activée par défaut pour les installations express et permet de s’assurer que votre version d’Azure AD Connecter est toujours à jour.
