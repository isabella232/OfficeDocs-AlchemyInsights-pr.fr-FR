---
title: Enregistrement des appels 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733847"
---
# <a name="11-call-recording"></a>Enregistrement des appels 1:1

Les administrateurs doivent prendre des mesures dès maintenant pour continuer à autoriser les utilisateurs à enregistrer les appels 1:1.
 
À compter du 12 avril 2021, nous allons commencer à appliquer une nouvelle option de stratégie d’appel Teams *AllowCloudRecordingForCalls*. 

Actuellement, les fonctionnalités d’enregistrement des appels 1:1 sont contrôlées par l’option *AllowCloudRecording* dans les stratégies de réunion Teams. Si vos utilisateurs sont autorisés à enregistrer des réunions Teams, ils peuvent également enregistrer des appels 1:1.

Si vous préférez empêcher tous les utilisateurs d’enregistrer des appels 1:1, aucune action n’est nécessaire. L’option de stratégie d’appel *AllowCloudRecordingForCalls* sera $False par défaut.

Cette modification est documentée dans la publication suivante du Centre de messages : (Mise à [jour) 1:1 Introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) de la stratégie d’enregistrement des appels pour définir l’option de stratégie d’appel Teams, vous devez utiliser Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

Pour activer l’enregistrement des appels dans les appels **1:1** : Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

Pour désactiver l’enregistrement des appels dans les appels **1:1** : Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

