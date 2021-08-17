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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886137"
---
# <a name="11-call-recording"></a>Enregistrement des appels 1:1

Si le **bouton Démarrer l’enregistrement** est grisé dans un appel 1:1, vous devez modifier les paramètres de stratégie pour l’utilisateur touché. Pour vérifier le paramètre de stratégie, exécutez diagnostic pour l’utilisateur touché en tapant **Diag: Teams 1:1 Call Recording** ci-dessus.     

À compter du 31 mai 2021, nous allons commencer à appliquer une nouvelle stratégie d’appel Teams *AllowCloudRecordingForCalls*. Avant cette modification, l’enregistrement des appels 1:1 est contrôlé par la stratégie de réunion Teams *AllowCloudRecording.* This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).  

*AllowCloudRecordingForCalls*   L’option de stratégie d’appel **est $False** par défaut. Si vous préférez empêcher tous les utilisateurs d’enregistrer des appels 1:1, aucune action n’est nécessaire.  

Pour activer l’enregistrement des appels pour tous les utilisateurs des appels 1:1, utilisez [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) pour exécuter l’cmdlet suivante : 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Vous pouvez également créer une stratégie et définir **-AllowCloudRecordingForCalls** sur **$true** et affecter cette stratégie à vos utilisateurs. 

Pour plus d’informations, voir [1:1 Call Recording Policy Controls Are (Almost!) Ici](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
