---
title: Outil d’exportation de la découverte électronique
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814586"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Vous ne pouvez pas installer ou exécuter l'outil d'exportation eDiscovery ?

Si vous ne pouvez pas installer ou exécuter l'outil d'exportation eDiscovery pour télécharger les résultats de recherche, vérifiez les points suivants :
  
- L'ordinateur que vous utilisez répond aux conditions préalables ci-après :

  - versions 32 ou 64 bits de Windows 7 et versions ultérieures

  - Microsoft .NET Framework 4.7

  - un navigateur pris en charge :

  - Microsoft Edge

    Ou

  - Internet Explorer 10 et versions ultérieures

    Les autres navigateurs, tels que Google Chrome et Mozilla Firefox, ne sont pas pris en charge.

- Votre organisation peut se connecter au point de terminaison dans Azure, qui est **\* .blob.core.windows.net** (le caractère générique représente un identificateur unique pour votre travail d'exportation).

- Le rôle Exporter vous est attribué dans le Centre de conformité de sécurité Microsoft 365. &amp; Par défaut, ce rôle est attribué uniquement au groupe de rôles Gestionnaire eDiscovery. Voir [Attribuer des autorisations eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Pour plus d'informations, [voir Exporter les résultats de la recherche de contenu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Si vous exportez plus de 100 000 boîtes aux lettres, vous devrez utiliser le Powershell suivant pour télécharger les résultats de l'exportation : Exportation des résultats de plus de  [100 000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)boîtes aux lettres.