---
title: Corriger les paramètres de stratégie/boîte aux lettres de l’utilisateur
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568497"
---
# <a name="fix-user-policymailbox-settings"></a>Corriger les paramètres de stratégie utilisateur/boîte aux lettres

Les paramètres de courrier indésirable de la boîte aux lettres ont affecté ce message. Pour passer en revue les paramètres, vous pouvez :

1. Lancez l’Exchange Management Shell. Pour plus d'informations, voir [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Exécutez cette commande (à l’aide de l’adresse e-mail de l’utilisateur)  **: get-mailboxjunkmailconfiguration -identity « user@domain.com »**
3. Vérifiez si l’adresse e-mail de l’expéditeur fait partie de **TrustedSendersAndDomains** ou **BlockedSendersAndDomains**. Si l’adresse de messagerie se trouve dans l’une des listes, vous de devez peut-être la supprimer. Pour plus d’informations, [voir Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
