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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682126"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Corriger les problèmes de remise des messages électroniques pour le code d’erreur 5.7.23

Vérifiez l’enregistrement DNS SPF pour votre domaine auprès d’un vérificateur d’enregistrement DNS ou SPF disponible publiquement sur le Web.

Vérifiez que le message sortant n’a pas été identifié comme courrier indésirable par Office 365 et routé via le [pool de remise à haut risque](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Les messages dans le pool de remise à haut risque ne passent pas les vérifications SPF, et par conséquent ne sont pas acceptés par l’organisation de messagerie de destination.

Si le problème persiste, contactez l’administrateur de l’hôte de messagerie auquel vous essayez d’envoyer des courriers électroniques. Notez l’erreur externe détaillée disponible dans le message de retour.  La prise en charge d’Office 365 peut ne pas être en mesure d’aider davantage.