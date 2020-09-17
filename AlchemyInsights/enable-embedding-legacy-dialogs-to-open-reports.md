---
title: Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806433"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports

**Symptôme**

Les utilisateurs ne peuvent pas ouvrir les rapports. « Une erreur s'est produite. Vérifiez les détails techniques pour en savoir plus. »

**Cause**

Échec de chargement des rapports dans UCI avec l’erreur « Le descripteur de formulaire est null ou n’est pas défini ». Les rapports dans UCI ont encore besoin de boîtes de dialogue héritées, de sorte que *allowlegacydialogsembedding* doit être activé sur le système du client.

**Solution**

1. Accédez à **Paramètres > Administration > Paramètres système > onglet Général**.

2. Définissez « Activer l’intégration de certaines boîtes de dialogue héritées dans le client du navigateur Unified Interface » sur **Oui**.
