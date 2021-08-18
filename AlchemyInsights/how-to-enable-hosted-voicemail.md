---
title: Comment activer la messagerie vocale hébergée
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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318646"
---
# <a name="how-to-enable-hosted-voicemail"></a>Comment activer la messagerie vocale hébergée

Pour activer la messagerie vocale, **HostedVoicemail** doit être $true.

Propriété **HostedVoicemail sur** l’utilisateur à l’aide de Remote PowerShell (RPS).

Pour plus d’informations sur la connexion au rps, voir Microsoft Teams vue d’ensemble de [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pour plus d’informations sur la connexion à RPS.

1. L’Teams administrateur doit être connecté à Remote PowerShell pour Teams.
1. À partir de PowerShell, invitez l’administrateur Teams peut exécuter **set-csuser user@contoso.com -HostedVoiceMail $true** où l’URI sip est de l’utilisateur en question.

**Remarque**: la réplication des modifications apportées aux stratégies peut prendre jusqu’à 24 heures.