---
title: Que faire si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603258"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Que faire si les fonctionnalités Azure ne fonctionnent pas correctement dans Microsoft Edge

Microsoft Edge présente des problèmes connus liés aux zones de sécurité qui peuvent affecter la façon dont les utilisateurs d'Azure se connectent au Centre d'administration Windows. Pour plus d’informations, reportez-vous à la rubrique [Problèmes connus sur Edge](https://go.microsoft.com/fwlink/?linkid=2140608). Si vous rencontrez des problèmes d’utilisation des fonctionnalités Azure avec Microsoft Edge, essayez ce qui suit :

1. Dans la menu Démarrer, dans la barre de **Recherche**, tapez **Options Internet**, puis sélectionnez-la.
1. Dans **Propriétés Internet**, sélectionnez l’onglet **Sécurité**.
1. Sélectionnez **Sites de confiance**, puis **Sites**.
1. Ajoutez l’URL de votre passerelle, ainsi que <https://login.microsoftonline.com> et <https://login.live.com>, puis sélectionnez **Fermer**.
1. Dans **Propriétés Internet**, sélectionnez l’onglet **Confidentialité**.
1. Dans la section Bloqueur de fenêtres contextuelles, sélectionnez **Paramètres**. Ajoutez votre URL de passerelle, ainsi que <https://login.microsoftonline.com> et <https://login.live.com>, puis sélectionnez **Fermer**.