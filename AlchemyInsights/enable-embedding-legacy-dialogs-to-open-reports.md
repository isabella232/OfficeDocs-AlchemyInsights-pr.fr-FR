---
title: Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003387"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports

**Symptôme**

Les utilisateurs ne peuvent pas ouvrir les rapports. « Une erreur s'est produite. Vérifiez les détails techniques pour en savoir plus. »

**Cause**

Échec de chargement des rapports dans UCI avec l’erreur « Le descripteur de formulaire est null ou n’est pas défini ». Les rapports dans UCI ont encore besoin de boîtes de dialogue héritées, de sorte que *allowlegacydialogsembedding* doit être activé sur le système du client.

**Solution**

1. Accédez à **Paramètres > Administration > Paramètres système > onglet Général**.

2. Définissez « Activer l’intégration de certaines boîtes de dialogue héritées dans le client du navigateur Unified Interface » sur **Oui**.
