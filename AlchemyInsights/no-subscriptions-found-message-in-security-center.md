---
title: Message Aucun abonnement trouvé dans le Centre de sécurité
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544106"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="0ecab-102">Message Aucun abonnement trouvé dans le Centre de sécurité</span><span class="sxs-lookup"><span data-stu-id="0ecab-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="0ecab-103">Si, en accédant au Centre de sécurité Microsoft Defender, vous obtenez le message «Aucun abonnement trouvé», cela signifie que l' Azure Active Directory (AAD) utilisé pour connecter l'utilisateur au portail ne possède pas de licence ATP Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="0ecab-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="0ecab-104">Les licences Windows E5 et Office E5 sont des licences distinctes.</span><span class="sxs-lookup"><span data-stu-id="0ecab-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="0ecab-p101">Ouvrez un dossier de support si la licence a été achetée mais n'a pas été provisionnée dans cette instance AAD. Soit vous avez :</span><span class="sxs-lookup"><span data-stu-id="0ecab-p101">Open a support case if the license was purchased but not provisioned to this AAD instance. Either you have:</span></span> <br/>
-   <span data-ttu-id="0ecab-107">Un problème éventuel d’approvisionnement de licence.</span><span class="sxs-lookup"><span data-stu-id="0ecab-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="0ecab-108">Vous avez approvisionné par inadvertance la licence à un autre Microsoft AAD que celui utilisé pour l’authentification auprès du service.</span><span class="sxs-lookup"><span data-stu-id="0ecab-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>