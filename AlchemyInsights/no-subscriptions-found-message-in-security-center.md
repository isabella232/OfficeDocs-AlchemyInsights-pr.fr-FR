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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768418"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>Message Aucun abonnement trouvé dans le Centre de sécurité

Si le message « Aucun abonnement trouvé » s’affiche lorsque vous accédez au Centre de sécurité Microsoft Defender, cela signifie que le compte DAS (Azure Active Directory) utilisé pour la connexion de l’utilisateur au portail ne possède pas de licence Microsoft Defender ATP.  

Les licences Windows E5 et Office E5 sont distinctes.

Ouvrez un cas de support si la licence a été achetée, mais n’a pas été approvisionnée pour cette instance AAD. Il peut s’agir de l’un des deux cas suivants : <br/>
-   Un problème éventuel d’approvisionnement de licence.<br/>
-   Vous avez approvisionné par inadvertance la licence à un autre Microsoft AAD que celui utilisé pour l’authentification auprès du service.