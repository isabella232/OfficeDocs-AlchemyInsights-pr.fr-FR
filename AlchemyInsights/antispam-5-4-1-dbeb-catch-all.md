---
title: Blocage du courrier indésirable 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717359"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Résolution des problèmes de remise pour le code d’erreur 550 5.4.1 accès au relais refusé

Ce problème se produit lorsque [vous vérifiez qu’une adresse de messagerie est valide pour empêcher bouncebacks lors de](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) l’entrée dans le réseau Microsoft. Procédez comme suit :

1. Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :
    - Domaine entier : parfois, le domaine doit être synchronisé ; essayez de [définir le domaine sur Internal, puis revenez à authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Adresse de messagerie unique : parfois, l’adresse doit être synchronisée ; Il est possible de modifier l’adresse proxy SMTP, puis de la modifier à nouveau.
2. Déterminez si le problème est spécifique à un groupe ou à un dossier public. Pour certains types d’objets, les objets doivent être créés manuellement dans Azure Active Directory.

Si vous avez besoin d’aide supplémentaire, ouvrez un ticket de support et spécifiez l’étendue du problème (y compris le type d’objet que vous envoyez) afin que nous puissions vous aider.