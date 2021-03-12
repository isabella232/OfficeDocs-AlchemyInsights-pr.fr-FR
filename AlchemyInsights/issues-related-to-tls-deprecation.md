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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="8d93a-102">Impossible d’envoyer/de recevoir du courrier électronique vers/depuis Office 365 en raison de la désactivation de TLS 1.0 et TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="8d93a-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="8d93a-103">Comme confirmé par le centre de messages après MC229914, l’arrêt de TLS 1.0 et TLS 1.1 a commencé à s’appliquer pour les points de terminaison de flux de messagerie Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="8d93a-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="8d93a-104">Bientôt, Office 365 n’acceptera plus les connexions de messagerie TLS 1.0 et TLS 1.1 provenant de sources externes.</span><span class="sxs-lookup"><span data-stu-id="8d93a-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="8d93a-105">En outre, Exchange Online n’utilisera jamais TLS 1.0 ou 1.1 pour envoyer des messages sortants.</span><span class="sxs-lookup"><span data-stu-id="8d93a-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="8d93a-106">Si vous êtes confronté à des problèmes en raison de la désactivation de TLS 1.0 ou 1.1, vous pouvez être confronté à l’une des erreurs suivantes :</span><span class="sxs-lookup"><span data-stu-id="8d93a-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="8d93a-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="8d93a-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="8d93a-108">Erreur dans l’Observateur de files d’attente du serveur local qui envoie du courrier électronique au responsable 365 - « 421 4.4.2 Connection dropped due to SocketError »</span><span class="sxs-lookup"><span data-stu-id="8d93a-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="8d93a-109">Erreur dans le journal [de](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) protocole du connecteur d’envoi sur le serveur envoyant du courrier électronique à Office 365 - Échec de la négociation TLS avec l’erreur SocketError</span><span class="sxs-lookup"><span data-stu-id="8d93a-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="8d93a-110">Erreur dans le journal de protocole du connecteur d’envoi ou de réception - « 451 5.7.3 Doit d’abord émettre une commande STARTTLS »</span><span class="sxs-lookup"><span data-stu-id="8d93a-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="8d93a-111">Si vous recevez l’une des erreurs ci-dessus, assurez-vous que TLS 1.2 est activé sur le serveur qui envoie ou reçoit des messages électroniques en vérifiant les clés de Registre suivantes :</span><span class="sxs-lookup"><span data-stu-id="8d93a-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="8d93a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **« DisabledByDefault"=dword:00000000 « Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **« DisabledByDefault"=dword:000000000 « Enabled"=dword:000000001**</span><span class="sxs-lookup"><span data-stu-id="8d93a-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="8d93a-113">Si vous modifiez les clés de Registre ci-dessus pour activer TLS 1.2, redémarrez le serveur pour que les modifications prennent effet.</span><span class="sxs-lookup"><span data-stu-id="8d93a-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="8d93a-114">Assurez-vous également que les dernières mises à jour Windows et Exchange sont installées.</span><span class="sxs-lookup"><span data-stu-id="8d93a-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="8d93a-115">Pour plus d’informations, consultez :</span><span class="sxs-lookup"><span data-stu-id="8d93a-115">For more information, see:</span></span>

- [<span data-ttu-id="8d93a-116">Exchange Server conseils TLS, partie 1 : Préparation de TLS 1.2 - Communauté technique Microsoft</span><span class="sxs-lookup"><span data-stu-id="8d93a-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="8d93a-117">Exchange Server conseils TLS partie 2 : activation de TLS 1.2 et identification des clients qui ne l’utilisent pas - Communauté technique Microsoft</span><span class="sxs-lookup"><span data-stu-id="8d93a-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="8d93a-118">Comprendre les scénarios de messagerie si les versions TLS ne peuvent pas être convenues avec Exchange Online - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="8d93a-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
