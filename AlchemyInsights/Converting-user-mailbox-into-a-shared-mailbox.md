---
title: Conversion d'une boîte aux lettres utilisateur en boîte aux lettres partagée?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374321"
---
Vous ne pouvez convertir une boîte aux lettres utilisateur en boîte aux lettres partagée que si l'utilisateur dispose d'une licence Exchange. Une fois la boîte aux lettres convertie, elle continue de s'afficher dans la liste des utilisateurs actifs, car cette liste inclut des boîtes aux lettres partagées. Toutefois, la boîte aux lettres convertie s'affiche également dans la liste des boîtes aux lettres partagées. 
  
Si vous essayez de convertir une boîte aux lettres dans la console d'administration Exchange et que la conversion échoue, effacez le cache et les cookies de votre navigateur, puis réessayez. Si cela ne fonctionne toujours pas, essayez de convertir la boîte aux lettres dans l'environnement de commande Exchange Management Shell en exécutant la commande suivante:
  
```
Set-Mailbox -Type Shared
```

D'autres informations de conversion de boîte aux lettres sont disponibles dans [convertir une boîte aux lettres utilisateur en boîte aux lettres partagée](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
