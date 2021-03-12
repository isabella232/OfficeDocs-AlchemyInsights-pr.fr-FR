---
title: Impossible d’envoyer/de recevoir du courrier électronique vers/depuis Office 365 en raison de la désactivation de TLS 1.0 et TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726919"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Impossible d’envoyer/de recevoir du courrier électronique vers/depuis Office 365 en raison de la désactivation de TLS 1.0 et TLS 1.1

Comme confirmé par le centre de messages après MC229914, l’arrêt de TLS 1.0 et TLS 1.1 a commencé à s’appliquer pour les points de terminaison de flux de messagerie Exchange Online. Bientôt, Office 365 n’acceptera plus les connexions de messagerie TLS 1.0 et TLS 1.1 provenant de sources externes. En outre, Exchange Online n’utilisera jamais TLS 1.0 ou 1.1 pour envoyer des messages sortants. Si vous êtes confronté à des problèmes en raison de la désactivation de TLS 1.0 ou 1.1, vous pouvez être confronté à l’une des erreurs suivantes :

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Erreur dans l’Observateur de files d’attente du serveur local qui envoie du courrier électronique au responsable 365 - « 421 4.4.2 Connection dropped due to SocketError »
- Erreur dans le journal [de](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) protocole du connecteur d’envoi sur le serveur envoyant du courrier électronique à Office 365 - Échec de la négociation TLS avec l’erreur SocketError
- Erreur dans le journal de protocole du connecteur d’envoi ou de réception - « 451 5.7.3 Doit d’abord émettre une commande STARTTLS »

Si vous recevez l’une des erreurs ci-dessus, assurez-vous que TLS 1.2 est activé sur le serveur qui envoie ou reçoit des messages électroniques en vérifiant les clés de Registre suivantes :

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **« DisabledByDefault"=dword:00000000 « Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **« DisabledByDefault"=dword:000000000 « Enabled"=dword:000000001**

Si vous modifiez les clés de Registre ci-dessus pour activer TLS 1.2, redémarrez le serveur pour que les modifications prennent effet. Assurez-vous également que les dernières mises à jour Windows et Exchange sont installées.

Pour plus d’informations, consultez :

- [Exchange Server conseils TLS, partie 1 : Préparation de TLS 1.2 - Communauté technique Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server conseils TLS partie 2 : activation de TLS 1.2 et identification des clients qui ne l’utilisent pas - Communauté technique Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Comprendre les scénarios de messagerie si les versions TLS ne peuvent pas être convenues avec Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
