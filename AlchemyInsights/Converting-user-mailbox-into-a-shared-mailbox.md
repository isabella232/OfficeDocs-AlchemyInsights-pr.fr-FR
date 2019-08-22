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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="f1c23-102">Convertir une boîte aux lettres d’utilisateur en boîte aux lettres partagée</span><span class="sxs-lookup"><span data-stu-id="f1c23-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="f1c23-103">Vous ne pouvez convertir une boîte aux lettres utilisateur en boîte aux lettres partagée que si l’utilisateur dispose d’une licence Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1c23-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="f1c23-104">Une fois la boîte aux lettres convertie, elle continue de s’afficher dans la liste des utilisateurs actifs, car cette liste inclut des boîtes aux lettres partagées.</span><span class="sxs-lookup"><span data-stu-id="f1c23-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="f1c23-105">Toutefois, la boîte aux lettres convertie s’affiche également dans la liste des boîtes aux lettres partagées.</span><span class="sxs-lookup"><span data-stu-id="f1c23-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="f1c23-106">Si vous essayez de convertir une boîte aux lettres dans la console d’administration Exchange et que la conversion échoue, effacez le cache et les cookies de votre navigateur, puis réessayez.</span><span class="sxs-lookup"><span data-stu-id="f1c23-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="f1c23-107">Si cela ne fonctionne toujours pas, essayez de convertir la boîte aux lettres dans l’environnement de commande Exchange Management Shell en exécutant la commande suivante:</span><span class="sxs-lookup"><span data-stu-id="f1c23-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="f1c23-108">D’autres informations de conversion de boîte aux lettres sont disponibles dans [convertir une boîte aux lettres utilisateur en boîte aux lettres partagée](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="f1c23-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
