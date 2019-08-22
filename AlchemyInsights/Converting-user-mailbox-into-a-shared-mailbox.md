---
title: Conversion d’une boîte aux lettres utilisateur en boîte aux lettres partagée?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496397"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Convertir une boîte aux lettres d’utilisateur en boîte aux lettres partagée

Vous ne pouvez convertir une boîte aux lettres utilisateur en boîte aux lettres partagée que si l’utilisateur dispose d’une licence Exchange. Une fois la boîte aux lettres convertie, elle continue de s’afficher dans la liste des utilisateurs actifs, car cette liste inclut des boîtes aux lettres partagées. Toutefois, la boîte aux lettres convertie s’affiche également dans la liste des boîtes aux lettres partagées. 
  
Si vous essayez de convertir une boîte aux lettres dans la console d’administration Exchange et que la conversion échoue, effacez le cache et les cookies de votre navigateur, puis réessayez. Si cela ne fonctionne toujours pas, essayez de convertir la boîte aux lettres dans l’environnement de commande Exchange Management Shell en exécutant la commande suivante:
  
```
Set-Mailbox -Type Shared
```

D’autres informations de conversion de boîte aux lettres sont disponibles dans [convertir une boîte aux lettres utilisateur en boîte aux lettres partagée](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
