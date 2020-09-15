---
title: Courrier indésirable-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717323"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corriger les problèmes de remise des messages électroniques pour le code d’erreur 5.7.23

Vérifiez l’enregistrement DNS SPF pour votre domaine auprès d’un vérificateur d’enregistrement DNS ou SPF disponible publiquement sur le Web.

Vérifiez que le message sortant n’a pas été identifié comme courrier indésirable par Microsoft et routé via le [pool de remise à haut risque](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Les messages dans le pool de remise à haut risque ne passent pas les vérifications SPF, et par conséquent ne sont pas acceptés par l’organisation de messagerie de destination.

Si le problème persiste, contactez l’administrateur de l’hôte de messagerie auquel vous essayez d’envoyer des courriers électroniques. Notez l’erreur externe détaillée disponible dans le message de retour. Le support Microsoft peut ne pas être en mesure d’aider plus en détail.
