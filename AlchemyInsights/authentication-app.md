---
title: Application d’authentification
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
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082940"
---
# <a name="authentication-app"></a>Application d’authentification

Si vous êtes un administrateur général, vous pouvez rapidement découvrir ce qui s’est passé ou diagnostiquer les problèmes liés à la connectez-vous à l’aide des [diagnostics de la signature.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Démarrez les diagnostics en cliquant sur le bouton «[Lancer le diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)». 
1. Recherchez l’événement à analyser en entrant les détails que vous avez sur l’utilisateur, l’application, l’heure de la signature, l’ID de demande ou l’ID de corrélation.
1. Examinez les résultats du diagnostic. Ils vous indiqueront ce qui s’est produit et les actions que vous pouvez prendre pour apporter des modifications, en cas de besoin.

**Vérifiez le scénario applicable :**

1. Si un utilisateur ne fait pas l’objet d’une notification Push dans l’application Microsoft Authenticator, vérifiez qu’il n’est pas affiché sous les utilisateurs bloqués par l’mf, comme décrit dans Bloquer et débloquer les [utilisateurs.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Si l’utilisateur n’est pas bloqué pour l' approbation MFA mais ne reçoit pas de notification Push, il peut ouvrir l’application Microsoft Authenticator, ce qui permet d’obtenir les demandes d’approbation en attente.
1. En tant qu’autre méthode de sign-in, l’utilisateur peut également cliquer sur Sign in another way et choisir d’utiliser un code de vérification à partir de mon application mobile.
1. L Microsoft Authenticator app est la seule méthode disponible pour de nombreux utilisateurs. [En savoir plus sur les paramètres de](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)sécurité par défaut, Authenticator faq sur l’application pour les questions fréquemment posées et comment les résoudre. [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)
 
**Vidéos recommandées**

[Comment configurer Authenticator App sur un nouveau téléphone (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
