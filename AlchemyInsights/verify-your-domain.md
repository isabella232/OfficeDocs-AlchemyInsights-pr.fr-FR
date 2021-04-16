---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770989"
---
# <a name="verify-your-domain"></a>Verify your domain

 **L'enregistrement n'a probablement pas été mis à jour sur Internet.**
  
En règle générale, nous ne pouvons voir le nouvel enregistrement que quelques minutes, mais cela peut parfois prendre jusqu'à quelques heures. 
  
- Si vous avez attendu aussi longtemps, vérifiez que vous avez copié et copié la valeur exacte dans l'enregistrement de vérification TXT de votre hôte DNS. Le problème vient souvent de l'omission de la portion « MS= » de l'enregistrement. Celle-ci est indispensable.

- Pour certains hôtes DNS, une étape supplémentaire est nécessaire pour enregistrer le fichier de zone (emplacement de stockage de l'enregistrement DNS) de façon à ce qu'il soit mis à jour sur Internet. Vérifiez que vous avez enregistré vos modifications afin que Microsoft puisse voir et vérifier l'enregistrement.
