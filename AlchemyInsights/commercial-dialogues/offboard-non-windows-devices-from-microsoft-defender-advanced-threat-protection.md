---
title: Hors-Windows à partir de Microsoft Defender – Protection avancée contre les menaces (ATP)
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967799"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Hors-Windows à partir de Microsoft Defender – Protection avancée contre les menaces (ATP)

Voici comment procéder :

1. Suivez la documentation tierce pour déconnecter la solution tierce de Microsoft Defender ATP.
2. À partir de Azure Active Directory client, supprimez les autorisations pour la solution tierce :

    1. Connectez-vous au [Portail Azure](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Sélectionnez **Tous les services**  >  **Azure Active Directory**  >  **Enterprise applications.**
    1. Sélectionnez l’application que vous souhaitez hors-carte.
    1. Sélectionnez **Supprimer**.

Pour plus d’informations, voir Les appareils [hors Windows.](https://go.microsoft.com/fwlink/?linkid=2143630)
