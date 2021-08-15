---
title: Appliquer automatiquement des étiquettes de niveau de sensibilité
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: 7a32ad52f115b9ada40f7cd47c90ceb3dcd3f9cd99a8f9eae3514b2e45e73bb8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969286"
---
# <a name="auto-apply-sensitivity-labels"></a>Appliquer automatiquement des étiquettes de niveau de sensibilité

Les étiquettes de sensibilité peuvent être appliquées manuellement au contenu par les utilisateurs, ou vous pouvez les configurer pour qu’elles soient automatiquement appliquées au contenu.

L’application automatique d’étiquettes de confidentialité supprime la nécessité de former les utilisateurs sur la façon de classifier le contenu et la nécessité de les informer des configurations de stratégie.

Pour appliquer automatiquement des étiquettes, les règles suivantes sont requises :

- Abonnement Azure Information Protection P2
- [Télécharger et installer le client d’étiquetage unifié Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

Nous travaillons sur la prise en charge native qui ne nécessitera pas le client d’étiquetage unifié Azure Information Protection à l’avenir.

Actuellement, seules Windows prend en charge le client d’étiquetage unifié.  La fonctionnalité n’est pas encore prise en charge sur Mac, iOS et Android.

Pour plus d’informations sur les étiquettes de niveau de sensibilité et leur application automatique au contenu, voir :

- [Vue d’ensemble des étiquettes de confidentialité](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [Appliquer automatiquement une étiquette de confidentialité à du contenu](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)