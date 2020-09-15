---
title: Problèmes liés à l’intégration d’ordinateurs
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676880"
---
# <a name="issues-with-onboarding-machines"></a>Problèmes liés à l’intégration d’ordinateurs

Il se peut que vous rencontriez des problèmes avec l’intégration d’ordinateurs au service MDATP. Si vous pouvez accéder à l’ordinateur de l’utilisateur final, procédez comme suit :

1. Téléchargez l’outil de diagnostic [Analyseur de connectivité client](https://aka.ms/mdatpanalyzer).
2. Faites l’extraction et exécutez MDATPAnalyzer.cmd.
3. Localisez le journal de diagnostic dans le dossier nommé MDATPClientAnalyzerResult, dossier identique à celui dans lequel l’outil Analyseur est téléchargé.
4. Examinez le fichier du journal, MDATPClientAnalyzer.txt, pour rechercher les problèmes de connectivité ou de paramètres de proxy Internet.