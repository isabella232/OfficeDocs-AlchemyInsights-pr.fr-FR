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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676495"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="a0132-102">Corriger les problèmes de remise des messages électroniques pour le code d’erreur 5.7.23</span><span class="sxs-lookup"><span data-stu-id="a0132-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="a0132-103">Vérifiez l’enregistrement DNS SPF pour votre domaine auprès d’un vérificateur d’enregistrement DNS ou SPF disponible publiquement sur le Web.</span><span class="sxs-lookup"><span data-stu-id="a0132-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="a0132-104">Vérifiez que le message sortant n’a pas été identifié comme courrier indésirable par Microsoft et routé via le [pool de remise à haut risque](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="a0132-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="a0132-105">Les messages dans le pool de remise à haut risque ne passent pas les vérifications SPF, et par conséquent ne sont pas acceptés par l’organisation de messagerie de destination.</span><span class="sxs-lookup"><span data-stu-id="a0132-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="a0132-106">Si le problème persiste, contactez l’administrateur de l’hôte de messagerie auquel vous essayez d’envoyer des courriers électroniques.</span><span class="sxs-lookup"><span data-stu-id="a0132-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="a0132-107">Notez l’erreur externe détaillée disponible dans le message de retour.</span><span class="sxs-lookup"><span data-stu-id="a0132-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="a0132-108">Le support Microsoft peut ne pas être en mesure d’aider plus en détail.</span><span class="sxs-lookup"><span data-stu-id="a0132-108">Microsoft support may not be able to assist further.</span></span>
