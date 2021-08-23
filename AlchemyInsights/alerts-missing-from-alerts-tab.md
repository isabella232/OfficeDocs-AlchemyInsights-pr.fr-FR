---
title: Alertes manquantes dans l’onglet Alertes
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362388"
---
# <a name="alerts-missing-from-alerts-tab"></a>Alertes manquantes dans l’onglet Alertes

**L’onglet Alertes** fonctionne en fonction de la configuration et des stratégies activées à partir du portail de gouvernance des applications de votre client. Les stratégies pré-actives dans la gouvernance des applications doivent également être activées pour que les signaux circulent vers **l’onglet Alertes.** 

Confirmez que l’alerte a été générée :

1. Go to app governance [Policies](https://compliance.microsoft.com/m365appprotection?viewid=policies) and confirm that you have created at least one Active or Audit policy.

1. Sélectionnez la stratégie, puis **modifiez-la** dans le volet volant. 

1. Vérifiez la configuration de la stratégie pour vérifier qu’une alerte doit avoir été générée en fonction d’un événement de stratégie initié il y a plus de 24 heures.

Pour plus d’informations sur les alertes dans la gouvernance des applications, voir La mise en place de la détection et de la correction des [menaces d’application.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)