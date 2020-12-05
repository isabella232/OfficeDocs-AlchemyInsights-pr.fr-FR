---
title: Procédure à suivre si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge
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
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576408"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Procédure à suivre si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge

Microsoft Edge présente des [problèmes connus](https://go.microsoft.com/fwlink/?linkid=2140608) liés aux zones de sécurité et peut influer sur la façon dont les utilisateurs Azure se connectent au centre d’administration Windows. Si vous rencontrez des problèmes lors de l’utilisation des fonctionnalités Azure avec Microsoft Edge, procédez comme suit :

1. Dans le menu **Démarrer** , recherchez **Options Internet** et sélectionnez-le.
2. Dans la boîte de dialogue **Propriétés Internet** , accédez à l’onglet **sécurité** .
3. Sélectionnez la zone **sites de confiance** , puis cliquez sur le bouton **sites** .
4. Dans la boîte de dialogue **sites de confiance** , ajoutez votre URL de passerelle, ainsi que [https://login.microsoftonline.com](https://login.microsoftonline.com) et, puis [https://login.live.com](https://login.live.com) sélectionnez **Fermer**.
5. Dans la boîte de dialogue **Propriétés Internet** , accédez à l’onglet **confidentialité** .
6. Dans la section **bloqueur de fenêtres publicitaires intempestives** , sélectionnez **paramètres**. Dans la boîte de dialogue qui s’ouvre, ajoutez votre URL de passerelle, ainsi que [https://login.microsoftonline.com](https://login.microsoftonline.com) et [https://login.live.com](https://login.live.com) , puis sélectionnez **Fermer**.
