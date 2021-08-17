---
title: 1332 OWA - Les règles de boîte de réception ne sont pas exécutées pour une boîte aux lettres
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040900"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Une règle de boîte de réception ne fonctionne pas comme prévu

Vérifiez les paramètres suivants dans Outlook sur le web :

- Un message peut être redirigé, transmis ou répondu automatiquement en fonction des règles de boîte de réception une seule fois. Une règle de redirection (règle de boîte de réception ou règle de flux de messagerie, également appelée règle de transport) peut ajouter un maximum de dix destinataires de redirection à un message. Pour plus d’informations, [consultez les limites](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)des règles de journal, de transport et de boîte de réception.

- Les règles de boîte de réception ne fonctionnent pas sur l’autre boîte aux lettres de journal. Pour plus d’informations sur l’autre boîte aux lettres de journaling, voir Autre boîte aux [lettres de journal.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Pour résoudre ces problèmes, [consultez la 2829319](https://support.microsoft.com/kb/2829319).

Si les problèmes précédents ne s’appliquent pas, exécutez le rapport de diagnostic des règles de boîte de réception avant de faire resserre le problème au Support Microsoft :

1. Ouvrez la boîte aux lettres Outlook sur le web, puis cliquez sur <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Paramètres**  >  **Afficher toutes les Outlook Paramètres**  >  **Courrier électronique**  >  **Règles**.

2. Au bas de la page, cliquez sur Si vos règles ne fonctionnent pas, cliquez ici **pour générer un rapport de diagnostic.**
