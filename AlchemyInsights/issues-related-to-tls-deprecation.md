---
title: Impossible d’envoyer/de recevoir des messages Office 365 en raison de la désactivation de TLS 1.0 et TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054904"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Impossible d’envoyer/de recevoir des messages Office 365 en raison de la désactivation de TLS 1.0 et TLS 1.1

Comme confirmé par le billet du centre de messages MC229914, l’arrêt de TLS 1.0 et TLS 1.1 a commencé à s’appliquer aux points de terminaison Exchange Online de flux de messagerie. Bientôt Office 365 n’acceptera plus les connexions de messagerie TLS 1.0 et TLS 1.1 provenant de sources externes. En outre, Exchange Online utilisera jamais TLS 1.0 ou 1.1 pour envoyer des messages sortants. Si vous êtes confronté à des problèmes en raison de la désactivation de TLS 1.0 ou 1.1, vous pouvez être confronté à l’une des erreurs suivantes :

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Erreur dans l’Observateur de files d’attente du serveur local qui envoie du courrier électronique au responsable 365 - « 421 4.4.2 Connection dropped due to SocketError »
- Erreur dans le journal [de](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) protocole du connecteur d’envoi sur le serveur envoyant des messages Office 365 - Échec de la négociation TLS avec l’erreur SocketError
- Erreur dans le journal de protocole du connecteur d’envoi ou de réception - « 451 5.7.3 Doit d’abord émettre une commande STARTTLS »

Si vous recevez l’une des erreurs ci-dessus, assurez-vous que TLS 1.2 est activé sur le serveur qui envoie ou reçoit des messages électroniques en vérifiant les clés de Registre suivantes :

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **« DisabledByDefault"=dword:00000000 « Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **« DisabledByDefault"=dword:00000000 « Enabled"=dword:00000001**

Si vous modifiez les clés de Registre ci-dessus pour activer TLS 1.2, redémarrez le serveur pour que les modifications prennent effet. Assurez-vous également que les dernières mises Windows et Exchange sont installées.

Pour plus d’informations, voir :

- [Exchange Server Conseils TLS, partie 1 : préparation pour TLS 1.2 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Conseils TLS Partie 2 : activation de TLS 1.2 et identification des clients qui ne l’utilisent pas - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Comprendre les scénarios de messagerie si les versions TLS ne peuvent pas être convenues avec Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
