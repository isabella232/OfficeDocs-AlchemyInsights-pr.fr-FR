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
# <a name="how-to-enable-hosted-voicemail"></a>Procédure d’activation de la messagerie vocale hébergée

Pour activer la messagerie vocale, **HostedVoicemail** doit être défini sur $true.

Propriété **HostedVoicemail** sur l’utilisateur à l’aide de PowerShell à distance (RPS).

Pour plus d’informations sur la connexion à RPS, reportez-vous à la rubrique [Microsoft teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pour plus d’informations sur la connexion à RPS.

1. L’administrateur teams doit être connecté à Remote PowerShell pour Teams.
1. À partir de l’invite PowerShell, l’administrateur de teams peut exécuter **Set-csuser user@contoso.com-HostedVoiceMail $true** où l’URI SIP est celui de l’utilisateur en question.

> [!NOTE]
> La réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.