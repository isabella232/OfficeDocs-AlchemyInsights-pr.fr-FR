---
title: Conversion des boîtes aux lettres de l’utilisateur dans une boîte aux lettres partagée ?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288724"
---
Vous pouvez convertir une boîte aux lettres de l’utilisateur à une boîte aux lettres partagée uniquement si l’utilisateur possède une licence Exchange. Une fois que la boîte aux lettres est converti, il continuera à afficher dans la liste d’utilisateurs actifs, car cette liste inclut des boîtes aux lettres partagées. Toutefois, la boîte aux lettres convertie également apparaîtront dans la liste de la boîte aux lettres partagée. 
  
Si vous tentez de convertir une boîte aux lettres dans la Console d’administration Exchange et l’échec de la conversion, désactivez le cache du navigateur et les cookies et réessayez. Si elle ne fonctionne pas, essayez de conversion de la boîte aux lettres dans Exchange Management Shell en exécutant la commande suivante :
  
```
Set-Mailbox -Type Shared
```

Plus d’informations sur la conversion boîte aux lettres sont disponibles dans [convertir une boîte aux lettres de l’utilisateur à une boîte aux lettres partagée](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
