---
title: Voulez-vous signaler un faux positif de courrier indésirable à Microsoft ?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396613"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Des messages légitimes sont marqués comme indésirables ?

C’est frustrant lorsqu’un e-mail légitime se retrouve dans le dossier Courrier indésirable ou en quarantaine. Considérez les raisons les plus courantes pour les faux positifs :

**Remplacements de client (les plus courants)** Il s’agit entièrement de votre contrôle pour la correction.

Envoyez le message sur Microsoft 365 Defender pour analyse des stratégies et règles qui ont un impact ; Les détails du rescan sont disponibles en quelques minutes.
Examinez ou modifiez les stratégies ou règles le cas échéant. 

**Remplacements par l’utilisateur final (courant)** Il s’agit entièrement de votre contrôle pour la correction. 

Envoyez le message sur Microsoft 365 Defender pour analyse des stratégies et règles qui ont un impact ; Les détails du rescan sont disponibles en quelques minutes. 

Si un message a été bloqué parce qu’il a été envoyé à partir d’une adresse de la liste des expéditeurs bloqués d’un utilisateur, les en-têtes incluent le verdict de filtrage du courrier indésirable « SFV:BLK ».

**Authentification du courrier électronique des expéditeurs** Il s’agit d’une partie de votre contrôle à corriger.

Envoyez le message pour analyser les échecs d’authentification de messagerie de l’expéditeur au moment de la remise . les résultats sont disponibles dans un jour. 

Si vous êtes propriétaire de l’infrastructure d’envoi, examinez comment l’aligner avec SPF, DKIM et DMARC pour vous assurer que les systèmes de messagerie de destination font confiance aux messages envoyés à partir de votre domaine. Vous pouvez également contacter les expéditeurs pour résoudre leurs configurations DNS.

**Verdicts de filtrage Microsoft** Il s’agit d’une partie de votre contrôle à corriger.

Soumettez le message et signalez-le comme étant sûr ; rescan results are available within a day. Utilisez la liste des locataires autoriser/bloquer lorsque vous n’êtes pas d’accord avec les verdicts de filtrage dans des situations particulières. Toutefois, vous ne devez pas contourner définitivement les verdicts de filtrage Microsoft. 

Pour plus d’informations, voir :

- Autorisez vos utilisateurs finaux à envoyer des messages à Microsoft. Microsoft utilise ces soumissions pour améliorer l’efficacité des technologies de protection de la messagerie, et elles apparaissent dans les rapports de soumission que vous pouvez utiliser comme indication pour mettre à jour les stratégies. 

- Pour regarder une courte vidéo sur l’envoi de messages pour analyse, voir [Envoi de messages pour analyse.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Utilisez la soumission de l’administrateur pour soumettre des courriers indésirables, l’hameçonnage, des URL et des fichiers à Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Gérer la liste Autoriser/Bloquer du client](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [En-têtes de message anti-courrier indésirable dans Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Protection contre le courrier indésirable sortant dans EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)