---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821409"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corriger les problèmes de remise des e-mails pour le code d'erreur 5.7.23

Vérifiez l'enregistrement DNS SPF pour votre domaine auprès d'un outil de vérification d'enregistrement SPF ou DNS disponible publiquement sur le web.

Vérifiez que le message sortant n'a pas été identifié comme courrier indésirable par Microsoft et acheminé via le pool de remise [à risque élevé.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Les messages du pool de remise à risque élevé ne sont pas acceptés par l'organisation de messagerie de destination et ne sont donc pas acceptés par l'organisation de messagerie de destination.

Si le problème persiste, vous devrez peut-être contacter l'administrateur de l'hôte de messagerie auquel vous tentez d'envoyer des messages électroniques. Notez l'erreur externe détaillée disponible dans la demande de non-lieu. Le support Microsoft peut ne pas être en mesure d'aider davantage.
