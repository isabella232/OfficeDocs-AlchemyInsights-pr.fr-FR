---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821445"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Corriger les problèmes de remise pour le code d'erreur 550 5.4.1 Accès au relais refusé

Ce problème se produit lors de la vérification de la validité d'une adresse de messagerie pour empêcher les [rebonds](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) lors de l'entrée sur le réseau Microsoft. Procédez comme suit :

1. Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :
    - Domaine entier : parfois, le domaine doit être synchronisé ; essayez [de définir le domaine sur Interne, puis revenir à Faisant autorité.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Adresse de messagerie unique : parfois, l'adresse doit être synchronisée . la modification de l'adresse proxy smtp et la modification de l'adresse de secours peuvent vous aider.
2. Déterminez si le problème est spécifique à un groupe ou un dossier public. Pour certains types d'objets, les objets devront peut-être être créés manuellement dans Azure Active Directory.

Si vous avez besoin d'aide supplémentaire, ouvrez un ticket de support et spécifiez l'étendue du problème (y compris le type d'objet à qui vous envoyez) afin que nous vous aidions mieux.