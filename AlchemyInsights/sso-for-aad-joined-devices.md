---
title: Single-Sign active pour les appareils joints à Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403796"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Sign-on unique pour les appareils joints à Azure Active Directory

Si vous avez un environnement Active Directory (AD) local et que vous souhaitez joindre vos ordinateurs joints à un domaine AD à Azure AD, vous pouvez le faire en rejoignant Azure AD hybride. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Configurer des appareils joints à Azure AD pour l'Single-Sign sur site à l’aide de Windows Hello Entreprise](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problèmes de jeton d’actualisation principal (PRT)** Un jeton d’actualisation principal (PRT) est un artefact clé de l’authentification Azure AD sur les appareils Windows 10, Windows Server 2016 et versions ultérieures, iOS et Android. Il s’agit d’un jeton web JSON (JWT) spécialement envoyé aux courtiers de jetons microsoft pour activer l' sign-on unique (SSO) sur les applications utilisées sur ces appareils. [Dans Qu’est-ce qu’un](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)jeton d’actualisation principal ? , nous fournirons des détails sur la façon dont un prt est émis, utilisé et protégé sur les appareils Windows 10.

**WamDefaultSet : OUI et AzureADPrt : OUI** Ces champs indiquent si l’utilisateur s’est authentifié avec succès à Azure AD lors de la signature de l’appareil. Si les valeurs sont **NO,** cela peut être dû :

- Clé de stockage non bonne dans le TPM associé à l’appareil lors de l’inscription (vérifiez keySignTest lors de l’exécution avec élévation de niveau).
- Autre ID de connexion
- Proxy HTTP in trouvé

Résoudre les problèmes d’appareils à l’aide de la commande dsregcmd - [État de l' sso](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
