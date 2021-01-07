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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "49768418"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="e1f7d-102">Message Aucun abonnement trouvé dans le Centre de sécurité</span><span class="sxs-lookup"><span data-stu-id="e1f7d-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="e1f7d-103">Si le message « Aucun abonnement trouvé » s’affiche lorsque vous accédez au Centre de sécurité Microsoft Defender, cela signifie que le compte DAS (Azure Active Directory) utilisé pour la connexion de l’utilisateur au portail ne possède pas de licence Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="e1f7d-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="e1f7d-104">Les licences Windows E5 et Office E5 sont distinctes.</span><span class="sxs-lookup"><span data-stu-id="e1f7d-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="e1f7d-105">Ouvrez un cas de support si la licence a été achetée, mais n’a pas été approvisionnée pour cette instance AAD.</span><span class="sxs-lookup"><span data-stu-id="e1f7d-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="e1f7d-106">Il peut s’agir de l’un des deux cas suivants :</span><span class="sxs-lookup"><span data-stu-id="e1f7d-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="e1f7d-107">Un problème éventuel d’approvisionnement de licence.</span><span class="sxs-lookup"><span data-stu-id="e1f7d-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="e1f7d-108">Vous avez approvisionné par inadvertance la licence à un autre Microsoft AAD que celui utilisé pour l’authentification auprès du service.</span><span class="sxs-lookup"><span data-stu-id="e1f7d-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>