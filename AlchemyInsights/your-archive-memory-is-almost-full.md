---
title: Votre boîte aux lettres d’archivage est presque pleine
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046750"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Votre boîte aux lettres d’archivage est presque pleine

Si l’utilisateur reçoit l’avertissement ; **Votre boîte aux lettres d’archivage est presque pleine** ou vous devez augmenter la taille de sa boîte aux lettres d’archivage, voici quelques conseils :

1. Si l’utilisateur se voit attribuer une licence Exchange Online Plan 1, mise à niveau vers **Exchange Online Plan 2** pour augmenter la taille de 50 Go à 100 Go.
1. Si l’utilisateur se voit déjà attribuer l’une des actions suivantes : **Exchange Online Plan 2** ou Exchange Online Plan 1 avec un module Archivage Exchange Online, utilisez les étapes ci-dessous pour activer l’archivage à extension automatique :
 
    1. [Connecter à Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Exécutez l’let de commande suivante pour l’utilisateur :  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Exécutez l’let de commande suivante pour vérifier qu’elle est activée pour l’utilisateur :  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Pour plus d’informations, voir :

- [Activer l’archivage illimité - Aide de l’administrateur - Microsoft 365 conformité | Documents Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online limites : descriptions de service | Documents Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Mettre à niveau vers une autre plan d'| Documents Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

