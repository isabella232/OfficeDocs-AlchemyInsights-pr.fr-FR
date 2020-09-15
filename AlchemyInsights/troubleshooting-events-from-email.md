---
title: Résolution des problèmes liés aux événements de courriers électroniques
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658732"
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