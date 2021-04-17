---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821445"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="a5e26-102">Corriger les problèmes de remise pour le code d'erreur 550 5.4.1 Accès au relais refusé</span><span class="sxs-lookup"><span data-stu-id="a5e26-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="a5e26-103">Ce problème se produit lors de la vérification de la validité d'une adresse de messagerie pour empêcher les [rebonds](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) lors de l'entrée sur le réseau Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5e26-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="a5e26-104">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a5e26-104">Try the following:</span></span>

1. <span data-ttu-id="a5e26-105">Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :</span><span class="sxs-lookup"><span data-stu-id="a5e26-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="a5e26-106">Domaine entier : parfois, le domaine doit être synchronisé ; essayez [de définir le domaine sur Interne, puis revenir à Faisant autorité.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="a5e26-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="a5e26-107">Adresse de messagerie unique : parfois, l'adresse doit être synchronisée . la modification de l'adresse proxy smtp et la modification de l'adresse de secours peuvent vous aider.</span><span class="sxs-lookup"><span data-stu-id="a5e26-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="a5e26-108">Déterminez si le problème est spécifique à un groupe ou un dossier public.</span><span class="sxs-lookup"><span data-stu-id="a5e26-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="a5e26-109">Pour certains types d'objets, les objets devront peut-être être créés manuellement dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a5e26-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="a5e26-110">Si vous avez besoin d'aide supplémentaire, ouvrez un ticket de support et spécifiez l'étendue du problème (y compris le type d'objet à qui vous envoyez) afin que nous vous aidions mieux.</span><span class="sxs-lookup"><span data-stu-id="a5e26-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>