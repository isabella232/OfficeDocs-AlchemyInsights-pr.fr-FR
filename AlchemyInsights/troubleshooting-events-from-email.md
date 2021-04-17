---
title: Résolution des problèmes liés aux événements de courriers électroniques
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834837"
---
# <a name="troubleshooting-events-from-email"></a>Résolution des problèmes liés aux événements de courriers électroniques

1. Vérifiez que la fonctionnalité est activée pour la boîte aux lettres : **Get-EventsFromEmailConfiguration-Identity <mailbox>**

2. Examinez ensuite les journaux « événements de la messagerie électronique » **Exporter-MailboxDiagnosticLogs <mailbox>-Composant TimeProfile**

3. Dans les journaux « Événements provenant de la messagerie », recherchez le InternetMessageId correspondant à l’élément dans la boîte aux lettres.  

4. La TrustScore détermine si l’élément est ajouté ou non. Les événements ne sont ajoutés que si TrustScore = « Approuvé ».

La TrustScore est déterminée par les propriétés SPF, Dkim ou Dmarc, qui se trouvent dans l’en-tête du message.

Pour afficher ces propriétés :

**Bureau Outlook**

- Ouvrir l’élément
- Fichier -> Propriétés -> en-têtes Internet

ou

**MFCMapi**

- Accéder à l’élément dans la boîte de réception
- Rechercher PR_TRANSPORT_MESSAGE_HEADERS_W

Ces propriétés sont déterminées et enregistrées pendant le transport et routage. Pour résoudre le problème, vous devrez peut-être suivre le support de transport relatif aux échecs dans SPF, DKIM et. ou DMARC.