---
title: Envoyer des notifications personnalisées avec Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086162"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Comment envoyer des notifications personnalisées aux utilisateurs d’appareils iOS et Android gérés

Les notifications personnalisées pour Intune sont traitées par l’Portail d’entreprise sur l’appareil d’un utilisateur. L’application crée ensuite la notification Push sur cet appareil.

Voici les conditions préalables de l’appareil pour prendre en charge la réception de notifications personnalisées, et pour que l’application crée ensuite la notification Push :

- L’appareil doit avoir l’Portail d’entreprise’application installée.  

- L’appareil doit autoriser l’application Portail d’entreprise envoyer des notifications Push. Lorsque l’application est installée ou mise à jour, elle invite l’utilisateur à autoriser les notifications.

- Google Play Services doit être installé sur les appareils Android.

- L’appareil doit être inscrit auprès d’Intune.

Pour plus d’informations, notamment sur l’envoi d’un message, voir la [documentation des fonctionnalités.](https://docs.microsoft.com/intune/custom-notifications)
