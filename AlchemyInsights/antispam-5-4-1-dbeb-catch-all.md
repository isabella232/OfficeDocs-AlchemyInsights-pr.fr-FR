---
title: Blocage du courrier indésirable 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964147"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Résolution des problèmes de remise pour le code d’erreur 550 5.4.1 accès au relais refusé

Ce problème se produit lorsque [vous vérifiez qu’une adresse de messagerie est valide pour empêcher bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) lors de l’entrée dans le réseau Office 365. Procédez comme suit :

1. Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :
    - Domaine entier : parfois, le domaine doit être synchronisé ; essayez de [définir le domaine sur Internal, puis revenez à authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Adresse de messagerie unique : parfois, l’adresse doit être synchronisée ; Il est possible de modifier l’adresse proxy SMTP, puis de la modifier à nouveau.
2. Déterminez si le problème est spécifique à un groupe ou à un dossier public. Pour certains types d’objets, les objets doivent être créés manuellement dans Azure Active Directory.

Si vous avez besoin d’aide supplémentaire, ouvrez un ticket de support et spécifiez l’étendue du problème (includidng le type d’objet vers lequel vous envoyez votre courrier) afin que nous puissions vous aider.