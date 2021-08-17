---
title: Connectez-vous Microsoft Edge manuellement
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f9aa27a585d805360e1fadecfd0db3b11d15a3594ed5bd5dc6c68cec37a4d6a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050764"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Connectez-vous Microsoft Edge manuellement

Si un utilisateur n’est pas automatiquement connecté lors d’une première utilisation, il peut se connecter manuellement via les paramètres du navigateur ou le volant d’identité. Pour gérer la connectez-vous, utilisez les stratégies suivantes :

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) : pour s’assurer qu’un utilisateur a toujours un profil de travail dans Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) : pour limiter la connectez-vous à un ensemble de comptes de confiance.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) : pour désactiver la sign-in ou pour forcer les utilisateurs à se connecter.

