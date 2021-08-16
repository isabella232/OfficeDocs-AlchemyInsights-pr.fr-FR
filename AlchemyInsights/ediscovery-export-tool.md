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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101300"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Vous ne pouvez pas installer ou exécuter l’outil d’exportation eDiscovery ?

Si vous ne pouvez pas installer ou exécuter l’outil d’exportation eDiscovery pour télécharger les résultats de recherche, vérifiez les points suivants :
  
- L’ordinateur que vous utilisez répond aux conditions préalables ci-après :

  - versions 32 ou 64 bits de Windows 7 et versions ultérieures

  - Microsoft .NET Framework 4.7.

  - Navigateur pris en charge :

  - Microsoft Edge

    Ou

  - Internet Explorer 10 et versions ultérieures

    Les autres navigateurs, tels que Google Chrome et Mozilla Firefox, ne sont pas pris en charge.

- Votre organisation peut se connecter au point de terminaison dans Azure, qui est **\* .blob.core.windows.net** (le caractère générique représente un identificateur unique pour votre travail d’exportation).

- Le rôle Exporter vous est attribué dans le Centre Microsoft 365 &amp; conformité de la sécurité. Par défaut, ce rôle est attribué uniquement au groupe de rôles Gestionnaire eDiscovery. Voir [Attribuer des autorisations eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Pour plus d’informations, [voir Exporter les résultats de la recherche de contenu.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Si vous exportez plus de 100 000 boîtes aux lettres, vous devez utiliser l’application Powershell suivante pour télécharger les résultats de l’exportation : Exportation des résultats de plus de  [100 000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)boîtes aux lettres.