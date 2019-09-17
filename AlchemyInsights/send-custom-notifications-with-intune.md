---
title: Envoyer des notifications personnalisées avec Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992311"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Comment envoyer des notifications personnalisées aux utilisateurs des appareils iOS et Android gérés

Les notifications personnalisées pour Intune sont traitées par l’application portail d’entreprise sur l’appareil d’un utilisateur. L’application crée ensuite la notification d’envoi sur cet appareil.

Voici les conditions préalables à l’appareil pour prendre en charge la réception de notifications personnalisées, et pour que l’application crée ensuite la notification d’envoi :

- L’application portail d’entreprise doit être installée sur l’appareil.  

- L’appareil doit permettre à l’application portail d’entreprise d’envoyer des notifications de type émission. Lorsque l’application est installée ou mise à jour, elle invite l’utilisateur à autoriser les notifications.

- Google Play services doit être installé sur les appareils Android.

- L’appareil doit être déployé avec Intune.

Pour plus d’informations sur l’envoi d’un message, consultez la documentation de la [fonctionnalité](https://docs.microsoft.com/intune/custom-notifications).
