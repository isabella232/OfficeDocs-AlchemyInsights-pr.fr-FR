---
title: Définir Microsoft Edge comme navigateur par défaut sur un appareil joint à un domaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426839"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a>Définir Microsoft Edge comme navigateur par défaut sur un appareil joint à un domaine

Définir Microsoft Edge comme navigateur par défaut : 

1. [Créez un fichier de configuration d’associations par défaut](https://go.microsoft.com/fwlink/?linkid=2132437) et stockez-le localement ou sur un partage réseau.

1. Ouvrez l’éditeur de stratégies de groupe, puis accédez à **Configuration d’un ordinateur** > **Modèlesodèles d’administration** > **Composants Windows** > **Explorateur de fichiers**.

1. Sélectionnez **Définir un fichier de configuration d’associations par défaut**.

1. Sélectionnez **Paramètre de stratégie**, puis sélectionnez **Activé**.

1. Sous **options**, entrez l’emplacement de votre fichier de configuration d’associations par défaut, puis sélectionnez **OK**.
