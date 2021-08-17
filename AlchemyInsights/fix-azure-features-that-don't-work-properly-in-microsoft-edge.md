---
title: Que faire si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117086"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Que faire si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge

Microsoft Edge [problèmes](https://go.microsoft.com/fwlink/?linkid=2140608) connus liés aux zones de sécurité et peuvent affecter la façon dont les utilisateurs Azure se connectent Windows Centre d’administration. Si vous avez des difficultés à utiliser les fonctionnalités Azure avec Microsoft Edge, essayez les étapes suivantes :

1. Dans le menu **Démarrer,** recherchez **options Internet** et sélectionnez-le.
2. Dans la boîte **de dialogue Propriétés Internet,** allez dans **l’onglet** Sécurité.
3. Sélectionnez la zone **Sites de** confiance, puis le bouton **Sites.**
4. Dans la **boîte de dialogue Sites** de confiance, ajoutez l’URL de votre passerelle, puis [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) sélectionnez **Fermer.**
5. Dans la boîte **de dialogue Propriétés Internet,** allez dans **l’onglet** Confidentialité.
6. Dans la section Bloqueur de fenêtres **pop-up,** **sélectionnez Paramètres**. Dans la boîte de dialogue qui s’ouvre, ajoutez l’URL de votre passerelle, puis [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) sélectionnez **Fermer.**
