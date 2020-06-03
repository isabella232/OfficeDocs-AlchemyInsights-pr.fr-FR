---
title: Courrier indésirable-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506441"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corriger les problèmes de remise des messages électroniques pour le code d’erreur 5.7.23

Vérifiez l’enregistrement DNS SPF pour votre domaine auprès d’un vérificateur d’enregistrement DNS ou SPF disponible publiquement sur le Web.

Vérifiez que le message sortant n’a pas été identifié comme courrier indésirable par Microsoft et routé via le [pool de remise à haut risque](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Les messages dans le pool de remise à haut risque ne passent pas les vérifications SPF, et par conséquent ne sont pas acceptés par l’organisation de messagerie de destination.

Si le problème persiste, contactez l’administrateur de l’hôte de messagerie auquel vous essayez d’envoyer des courriers électroniques. Notez l’erreur externe détaillée disponible dans le message de retour. Le support Microsoft peut ne pas être en mesure d’aider plus en détail.
