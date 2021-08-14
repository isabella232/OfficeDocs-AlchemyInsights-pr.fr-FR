---
title: Erreurs de connexion d’un utilisateur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 09950bcbc96c95caff0d7b1b7c98373360a9900cd01fd6faf9e787f67cefb5a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53990489"
---
# <a name="user-sign-in-errors"></a>Erreurs de connexion d’un utilisateur

**Résoudre les problèmes avec le diagnostic de connexion**

Pour détecter la cause ou diagnostiquer les problèmes liés à la connexion de l’utilisateur, effectuez ces étapes :

1. Lancez le [diagnostic de connexion](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Recherchez l’événement à analyser en entrant les informations dont vous disposez sur l’utilisateur, l’application, l’heure de la connexion, l’ID de requête ou l’ID de corrélation.
3. Examinez les résultats de diagnostic en indiquant les détails de ce qui s’est produit et les actions que vous pouvez prendre pour apporter des modifications, si des modifications sont nécessaires.

**Recherchez-vous des informations sur les codes d’erreur AADSTS renvoyés à partir du service de jeton de sécurité Azure Active Directory (Azure AD) ?** Lisez [cet article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pour trouver des descriptions  d’erreurs AADSTS, des correctifs et quelques solutions de contournement suggérées