---
title: Problèmes d’accès conditionnel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069962"
---
# <a name="conditional-access-issues"></a>Problèmes d’accès conditionnel

**Résoudre les problèmes avec le diagnostic de connexion**

Vous pouvez rapidement découvrir ce qui s’est passé ou diagnostiquer les problèmes liés à la connectez-vous à l’aide du [diagnostic de la sign-in](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Lancez le diagnostic de connexion.
1. Recherchez l’événement à analyser en entrant les détails que vous avez sur l’utilisateur, l’application, l’heure de la signature, l’ID de demande ou l’ID de corrélation.
1. Examinez les résultats de diagnostic montrant les détails de ce qui s’est passé et les actions que vous pouvez prendre pour apporter des modifications (si des modifications sont nécessaires).

**Étapes pour résoudre les problèmes de la sign-in** 

1. Accédez à la page de signature Azure AD.
1. Filtrer les connecteurs par utilisateur, plage de temps, application, état, application cliente, etc.
1. Sélectionnez un événement de sign-in et affichez l’onglet Accès conditionnel pour voir quelles stratégies ont été évaluées.
1. Cliquez sur la ligne d’une stratégie pour afficher les détails de la stratégie et comprendre pourquoi elle a été appliquée.

**Outils permettant de résoudre les problèmes d’une stratégie d’accès conditionnel**

- Le mode Rapport uniquement vous permet d’évaluer une stratégie sans impact sur les utilisateurs.
- L’outil De simulation vous permet de simuler des événements de sign-in et de voir quelles stratégies s’appliquent.
- Informations de rapports affiche l’impact en temps réel de chaque stratégie.

**Stratégies de protection de référence**

Les stratégies de protection de référence ont été dépréciées. Elles ne sont plus appliquées et seront bientôt supprimées du portail Azure. Nous vous recommandons d’activer [les paramètres de sécurité par défaut.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Pour plus d’informations sur l’accès conditionnel, voir :

[Meilleures pratiques en matière d’accès conditionnel dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions de l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Contrôles dans l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Emplacements dans l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
