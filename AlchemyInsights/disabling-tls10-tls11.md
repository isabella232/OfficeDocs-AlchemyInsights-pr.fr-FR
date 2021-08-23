---
title: Désactivation de TLS1.0 et TLS 1.1 pour l’envoi du client SMTP AUTH
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/18/2021
ms.locfileid: "58380671"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>Désactivation de TLS1.0 et TLS 1.1 pour l’envoi du client SMTP AUTH

Nous avons récemment commencé à désactiver TLS1.0 et TLS 1.1 pour l’envoi de client SMTP AUTH. 

Si vous avez configuré un appareil, une application ou un serveur qui envoie des e-mails à Microsoft 365 à l’aide de la méthode de soumission du client AUTH SMTP, assurez-vous que votre appareil, votre application ou votre serveur prend en charge TLS 1.2 pour SMTP. 