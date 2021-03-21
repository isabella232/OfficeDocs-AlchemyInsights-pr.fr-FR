---
title: Protection contre les attaques de rétrodiffusion
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897705"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="ed5c4-102">Protection contre les attaques de rétrodiffusion</span><span class="sxs-lookup"><span data-stu-id="ed5c4-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="ed5c4-103">La rétrodiffusion est les rapports d’erreur de remise (également appelés rapports d’erreur ou messages de non-remise) que vous recevez pour les messages que vous n’avez pas envoyés.</span><span class="sxs-lookup"><span data-stu-id="ed5c4-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="ed5c4-104">Les expéditeurs de courrier indésirable falsifient (usurpent) l’adresse **De :** de leurs messages. Ils utilisent souvent des adresses de messagerie réelles pour donner de la crédibilité à leurs messages.</span><span class="sxs-lookup"><span data-stu-id="ed5c4-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="ed5c4-105">Par conséquent, lorsque les expéditeurs de courrier indésirable envoient inévitablement des messages à des destinataires inexistants, le serveur de messagerie de destination est essentiellement piégé et renvoie le message non distribuable dans un NDR à l'expéditeur falsifié dans l'adresse **De :** .</span><span class="sxs-lookup"><span data-stu-id="ed5c4-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="ed5c4-106">Des informations supplémentaires sont disponibles dans la [Rétrodiffusion dans EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="ed5c4-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="ed5c4-107">**Activation de la protection contre la rétrodiffusion**</span><span class="sxs-lookup"><span data-stu-id="ed5c4-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="ed5c4-108">Pour activer la protection contre la rétrodiffusion, suivez le chemin d’accès ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="ed5c4-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="ed5c4-109">**protection.office.com > Gestion des menaces > Stratégie > Anti-courrier indésirable > Sélectionner la stratégie de filtrage du courrier indésirable et modifier la stratégie > Propriétés du courrier indésirable > Marquer comme courrier indésirable > Rétrodiffusion NDR > Définir sur « Activé »**</span><span class="sxs-lookup"><span data-stu-id="ed5c4-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="ed5c4-110">Si vous pensez qu’un compte a été compromis, consultez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="ed5c4-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="ed5c4-111">Répondre à un compte d'e-mail compromis</span><span class="sxs-lookup"><span data-stu-id="ed5c4-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="ed5c4-112">Suppression d’utilisateurs bloqués du portail Utilisateurs restreints dans Office 365</span><span class="sxs-lookup"><span data-stu-id="ed5c4-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



