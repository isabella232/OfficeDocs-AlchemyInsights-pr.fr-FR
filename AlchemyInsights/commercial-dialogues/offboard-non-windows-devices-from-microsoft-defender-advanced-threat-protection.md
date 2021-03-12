---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735927"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)

Voici comment procéder :

1. Suivez la documentation tierce pour déconnecter la solution tierce de Microsoft Defender ATP.
2. À partir de votre client Azure Active Directory, supprimez les autorisations pour la solution tierce :

    1. Connectez-vous au [portail Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Sélectionnez **tous les services** Azure Active  >  **Directory** Enterprise  >  **Applications**.
    1. Sélectionnez l’application que vous souhaitez horsboard.
    1. Sélectionnez **Supprimer**.

Pour en savoir plus, consultez [Les appareils hors](https://go.microsoft.com/fwlink/?linkid=2143630)Windows.
