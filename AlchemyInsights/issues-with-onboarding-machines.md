---
title: Problèmes liés à l’intégration d’ordinateurs
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139024"
---
# <a name="issues-with-onboarding-machines"></a>Problèmes liés à l’intégration d’ordinateurs

Il se peut que vous rencontriez des problèmes avec l’intégration d’ordinateurs au service MDATP. Si vous pouvez accéder à l’ordinateur de l’utilisateur final, procédez comme suit :

1. Téléchargez l’outil de diagnostic [Analyseur de connectivité client](https://aka.ms/mdatpanalyzer).
2. Faites l’extraction et exécutez MDATPAnalyzer.cmd.
3. Localisez le journal de diagnostic dans le dossier nommé MDATPClientAnalyzerResult, dossier identique à celui dans lequel l’outil Analyseur est téléchargé.
4. Examinez le fichier du journal, MDATPClientAnalyzer.txt, pour rechercher les problèmes de connectivité ou de paramètres de proxy Internet.