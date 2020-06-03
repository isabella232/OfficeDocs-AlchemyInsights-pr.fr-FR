---
title: Outil d’exportation de la découverte électronique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 6352603a391ddcb44d2728c7587bf15a6cd97ebb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507168"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Vous ne parvenez pas à installer ou exécuter l’outil d’exportation de découverte électronique ?

Si vous ne pouvez pas installer ou exécuter l’outil d’exportation de découverte électronique pour télécharger les résultats de la recherche, vérifiez les points suivants :
  
- L’ordinateur que vous utilisez répond aux conditions préalables suivantes :

  - versions 32 ou 64 bits de Windows 7 et versions ultérieures

  - Microsoft .NET Framework 4,7

  - un navigateur pris en charge :

  - Microsoft Edge

    Ou

  - Internet Explorer 10 et versions ultérieures

    D’autres navigateurs, tels que Google Chrome et Mozilla Firefox ne sont pas pris en charge.

- Votre organisation peut se connecter au point de terminaison dans Azure, c’est-à-dire ** \* . blob.Core.Windows.net** (le caractère générique représente un identificateur unique pour votre tâche d’exportation).

- Vous avez reçu le rôle d’exportation dans le centre de sécurité conformité Microsoft 365 &amp; . Par défaut, ce rôle est uniquement attribué au groupe de rôles gestionnaire eDiscovery. Consultez la rubrique [attribution d’autorisations eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Pour plus d’informations, consultez la rubrique [exporter des résultats de recherche de contenu](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  