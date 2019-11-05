---
title: Blocage du courrier indésirable 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964147"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="14cc7-102">Résolution des problèmes de remise pour le code d’erreur 550 5.4.1 accès au relais refusé</span><span class="sxs-lookup"><span data-stu-id="14cc7-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="14cc7-103">Ce problème se produit lorsque [vous vérifiez qu’une adresse de messagerie est valide pour empêcher bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) lors de l’entrée dans le réseau Office 365.</span><span class="sxs-lookup"><span data-stu-id="14cc7-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="14cc7-104">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="14cc7-104">Try the following:</span></span>

1. <span data-ttu-id="14cc7-105">Déterminez si le problème est spécifique à un domaine entier ou à une adresse de messagerie unique :</span><span class="sxs-lookup"><span data-stu-id="14cc7-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="14cc7-106">Domaine entier : parfois, le domaine doit être synchronisé ; essayez de [définir le domaine sur Internal, puis revenez à authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="14cc7-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="14cc7-107">Adresse de messagerie unique : parfois, l’adresse doit être synchronisée ; Il est possible de modifier l’adresse proxy SMTP, puis de la modifier à nouveau.</span><span class="sxs-lookup"><span data-stu-id="14cc7-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="14cc7-108">Déterminez si le problème est spécifique à un groupe ou à un dossier public.</span><span class="sxs-lookup"><span data-stu-id="14cc7-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="14cc7-109">Pour certains types d’objets, les objets doivent être créés manuellement dans Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14cc7-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="14cc7-110">Si vous avez besoin d’aide supplémentaire, ouvrez un ticket de support et spécifiez l’étendue du problème (includidng le type d’objet vers lequel vous envoyez votre courrier) afin que nous puissions vous aider.</span><span class="sxs-lookup"><span data-stu-id="14cc7-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>