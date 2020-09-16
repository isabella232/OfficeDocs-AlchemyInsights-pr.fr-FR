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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720644"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Comment envoyer des notifications personnalisées aux utilisateurs des appareils iOS et Android gérés

Les notifications personnalisées pour Intune sont traitées par l’application portail d’entreprise sur l’appareil d’un utilisateur. L’application crée ensuite la notification d’envoi sur cet appareil.

Voici les conditions préalables à l’appareil pour prendre en charge la réception de notifications personnalisées, et pour que l’application crée ensuite la notification d’envoi :

- L’application portail d’entreprise doit être installée sur l’appareil.  

- L’appareil doit permettre à l’application portail d’entreprise d’envoyer des notifications de type émission. Lorsque l’application est installée ou mise à jour, elle invite l’utilisateur à autoriser les notifications.

- Google Play services doit être installé sur les appareils Android.

- L’appareil doit être déployé avec Intune.

Pour plus d’informations sur l’envoi d’un message, consultez la documentation de la [fonctionnalité](https://docs.microsoft.com/intune/custom-notifications).
