---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734304"
---
# <a name="verify-your-domain"></a>Verify your domain

 **L’enregistrement n’a probablement pas été mis à jour sur Internet.**
  
En règle générale, il ne prend que quelques minutes pour pouvoir voir le nouvel enregistrement, mais il peut arriver que quelques heures se soient nécessaires. 
  
- Si vous avez attendu une fois déjà, vérifiez que vous avez copié et collé la valeur exacte dans l’enregistrement de vérification TXT au niveau de votre hôte DNS. Le problème vient souvent de l'omission de la portion « MS= » de l'enregistrement. Celle-ci est indispensable.

- Pour certains hôtes DNS, une étape supplémentaire est nécessaire pour enregistrer le fichier de zone (emplacement de stockage de l'enregistrement DNS) de façon à ce qu'il soit mis à jour sur Internet. Assurez-vous que vous avez enregistré vos modifications afin que Microsoft puisse voir et vérifier l’enregistrement.
