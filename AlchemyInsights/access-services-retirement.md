---
title: Déclassement Access services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050487"
---
# <a name="access-services-retirement"></a>Déclassement Access services

Comme nous l’avons annoncé à l’origine dans MC97576, en mars 2017, et continuait de communiquer au cours de l’année précédente, Access services est retiré de Office 365. La phase suivante de ce processus est la suppression des bases de données Web Access qui utilisent des listes SharePoint comme stockage de données sous-jacent.

**Comment cela m’affecte-t-il ?**

À partir du 2019 juin, nous allons arrêter la création de nouvelles bases de données Access dans SharePoint Online et arrêter le service et toutes les applications restantes d’avril 2020.

**Que dois-je faire pour préparer cette modification ?**

Nous vous encourageons à créer un plan de transition pour les bases de données Web Access de votre organisation. Les administrateurs peuvent utiliser l' [analyseur d’applications SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pour obtenir un inventaire des applications Access que les sites utilisent.

Il existe plusieurs façons de migrer des données de bases de données Web Access :

- Importation dans une base de données Access locale (. ACCDB) ou dans un fichier Excel.
- Nous vous recommandons également d’explorer Microsoft PowerApps comme une autre plate-forme pour créer des solutions d’entreprise sans code pour le Web et les appareils mobiles.