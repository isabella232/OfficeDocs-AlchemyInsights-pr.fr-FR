---
title: Message Aucun abonnement trouvé dans le Centre de sécurité
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544106"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Message Aucun abonnement trouvé dans le Centre de sécurité

Si, en accédant au Centre de sécurité Microsoft Defender, vous obtenez le message «Aucun abonnement trouvé», cela signifie que l' Azure Active Directory (AAD) utilisé pour connecter l'utilisateur au portail ne possède pas de licence ATP Microsoft Defender.  

Les licences Windows E5 et Office E5 sont des licences distinctes.

Ouvrez un dossier de support si la licence a été achetée mais n'a pas été provisionnée dans cette instance AAD. Soit vous avez : <br/>
-   Un problème éventuel d’approvisionnement de licence.<br/>
-   Vous avez approvisionné par inadvertance la licence à un autre Microsoft AAD que celui utilisé pour l’authentification auprès du service.