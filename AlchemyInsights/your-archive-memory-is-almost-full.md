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
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950507"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Votre boîte aux lettres d’archivage est presque pleine

Si l’utilisateur reçoit l’avertissement ; **Votre boîte aux lettres d’archivage est presque pleine** ou vous devez augmenter la taille de sa boîte aux lettres d’archivage, voici quelques conseils :

1. Si une licence Exchange Online Plan 1 est attribuée à l’utilisateur, mise à niveau vers **Exchange Online Plan 2** pour augmenter la taille de 50 Go à 100 Go.
1. Si l’utilisateur est déjà affecté à l’un des services suivants : **Exchange Online Plan 2** ou Exchange Online Plan 1 avec un module Archivage Exchange Online, utilisez les étapes ci-dessous pour activer l’archivage à extension automatique :
 
    1. [Connectez-vous à Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Exécutez l’let de commande suivante pour l’utilisateur :  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Exécutez l’let de commande suivante pour vérifier qu’elle est activée pour l’utilisateur :  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Pour plus d'informations, consultez les rubriques suivantes :

- [ Activer l’archivage illimité - Aide de l’administrateur - Microsoft 365 Compliance | Documents Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limites d’Exchange Online : descriptions de service | Documents Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Mettre à niveau vers une autre plan d'| Documents Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

