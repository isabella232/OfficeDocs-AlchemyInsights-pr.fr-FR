---
title: Procédure d’activation de la messagerie vocale hébergée
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608850"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="82e2e-102">Procédure d’activation de la messagerie vocale hébergée</span><span class="sxs-lookup"><span data-stu-id="82e2e-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="82e2e-103">Pour activer la messagerie vocale, **HostedVoicemail** doit être défini sur $true.</span><span class="sxs-lookup"><span data-stu-id="82e2e-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="82e2e-104">Propriété **HostedVoicemail** sur l’utilisateur à l’aide de PowerShell à distance (RPS).</span><span class="sxs-lookup"><span data-stu-id="82e2e-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="82e2e-105">Pour plus d’informations sur la connexion à RPS, reportez-vous à la rubrique [Microsoft teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pour plus d’informations sur la connexion à RPS.</span><span class="sxs-lookup"><span data-stu-id="82e2e-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="82e2e-106">L’administrateur teams doit être connecté à Remote PowerShell pour Teams.</span><span class="sxs-lookup"><span data-stu-id="82e2e-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="82e2e-107">À partir de l’invite PowerShell, l’administrateur de teams peut exécuter **Set-csuser user@contoso.com-HostedVoiceMail $true** où l’URI SIP est celui de l’utilisateur en question.</span><span class="sxs-lookup"><span data-stu-id="82e2e-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="82e2e-108">La réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.</span><span class="sxs-lookup"><span data-stu-id="82e2e-108">Changes to policies can take up to 24 hours to replicate.</span></span>