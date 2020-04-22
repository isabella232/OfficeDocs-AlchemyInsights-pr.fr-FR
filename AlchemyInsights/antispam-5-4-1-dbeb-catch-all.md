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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707909"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Résolution des problèmes de remise pour le code d’erreur 550 5.4.1 accès au relais refusé

Ce problème se produit lorsque [vous vérifiez qu’une adresse de messagerie est valide pour empêcher bouncebacks lors de](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) l’entrée dans le réseau Microsoft. Procédez comme suit :

1. Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :
    - Domaine entier : parfois, le domaine doit être synchronisé ; essayez de [définir le domaine sur Internal, puis revenez à authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Adresse de messagerie unique : parfois, l’adresse doit être synchronisée ; Il est possible de modifier l’adresse proxy SMTP, puis de la modifier à nouveau.
2. Déterminez si le problème est spécifique à un groupe ou à un dossier public. Pour certains types d’objets, les objets doivent être créés manuellement dans Azure Active Directory.

Si vous avez besoin d’aide supplémentaire, ouvrez un ticket de support et spécifiez l’étendue du problème (y compris le type d’objet que vous envoyez) afin que nous puissions vous aider.