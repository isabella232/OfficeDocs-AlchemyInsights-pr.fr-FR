---
title: Conversion des boîtes aux lettres de l’utilisateur dans une boîte aux lettres partagée ?
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906730"
---
Vous pouvez convertir une boîte aux lettres de l’utilisateur à une boîte aux lettres partagée uniquement si l’utilisateur possède une licence Exchange. Une fois que la boîte aux lettres est converti, il continuera à afficher dans la liste d’utilisateurs actifs, car cette liste inclut des boîtes aux lettres partagées. Toutefois, la boîte aux lettres convertie également apparaîtront dans la liste de la boîte aux lettres partagée. 
  
Si vous tentez de convertir une boîte aux lettres dans la Console d’administration Exchange et l’échec de la conversion, désactivez le cache du navigateur et les cookies et réessayez. Si elle ne fonctionne pas, essayez de conversion de la boîte aux lettres dans Exchange Management Shell en exécutant la commande suivante :
  
```
Set-Mailbox -Type Shared
```

Plus d’informations sur la conversion boîte aux lettres sont disponibles dans [convertir une boîte aux lettres de l’utilisateur à une boîte aux lettres partagée](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
