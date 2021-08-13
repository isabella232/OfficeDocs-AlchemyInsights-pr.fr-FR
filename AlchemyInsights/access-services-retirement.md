---
title: Retrait des services Access
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938693"
---
# <a name="access-services-retirement"></a>Retrait des services Access

Comme nous l’avons initialement annoncé dans MC97576, en mars 2017, et que nous avons continué à communiquer au cours de l’année Access Services sont retirés. La phase suivante de ce processus sera la suppression des bases de données Web Access qui utilisent des listes SharePoint comme stockage de données sous-jacent.

**En quoi cela m’affecte-t-il ?**

À compter de juin 2019, nous arrêterons la création de nouvelles bases de données Access dans SharePoint Online et arrêterons le service et toutes les applications restantes d’avril 2020.

**Que dois-je faire pour me préparer à ce changement ?**

Nous vous encourageons à créer un plan de transition pour les bases de données web Access de votre organisation. Les administrateurs peuvent utiliser le [scanneur SharePoint’application Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pour obtenir un inventaire des applications Access utilisées par les sites.

Il existe plusieurs façons de migrer les données des bases de données web Access :

- Importation dans une base de données Access locale (. ACCDB) ou à un fichier Excel’accès.
- Nous vous recommandons également d’explorer Microsoft PowerApps comme plateforme alternative pour créer des solutions métier sans code pour les appareils web et mobiles.