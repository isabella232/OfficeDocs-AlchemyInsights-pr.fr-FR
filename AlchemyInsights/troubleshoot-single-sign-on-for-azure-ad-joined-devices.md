---
title: Résoudre les problèmes d' sign-on unique pour les appareils joints à Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039244"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Résoudre les problèmes d' sign-on unique pour les appareils joints à Azure AD

Si vous avez un environnement Active Directory (AD) local et que vous souhaitez joindre vos ordinateurs joints à un domaine AD à Azure AD, vous pouvez le faire en rejoignant Azure AD hybride. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

Pour plus d’informations, voir Configurer les appareils joints à [Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)pour l'Single-Sign local à l’aide Windows Hello entreprise.

**Problèmes de jeton d’actualisation principal (PRT)**

Un jeton d’actualisation principal (PRT) est un artefact clé de l’authentification Azure AD sur les appareils Windows 10, Windows Server 2016 et versions ultérieures, iOS et Android. Il s’agit d’un jeton web JSON (JWT) spécialement envoyé aux courtiers de jetons microsoft pour activer l' sign-on unique (SSO) sur les applications utilisées sur ces appareils. Pour plus d’informations sur la façon dont un PRT est émis, utilisé et protégé sur les appareils Windows 10, voir Qu’est-ce qu’un jeton d’actualisation [principal ?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet : OUI et AzureADPrt : OUI**

Ces champs indiquent si l’utilisateur s’est authentifié avec succès à Azure AD lors de la signature de l’appareil. Si les valeurs sont **NO,** cela peut être dû à :

- Clé de stockage non bonne dans le TPM associé à l’appareil lors de l’inscription (vérifiez keySignTest lors de l’exécution avec élévation de niveau)
- Autre ID de connexion
- Proxy HTTP in trouvé

Pour résoudre les problèmes d’appareils à l’aide de la commande dsregcmd, consultez [l’état de l' cesso.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
