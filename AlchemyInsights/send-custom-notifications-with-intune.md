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
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="27eb6-102">Comment envoyer des notifications personnalisées aux utilisateurs des appareils iOS et Android gérés</span><span class="sxs-lookup"><span data-stu-id="27eb6-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="27eb6-103">Les notifications personnalisées pour Intune sont traitées par l’application portail d’entreprise sur l’appareil d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="27eb6-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="27eb6-104">L’application crée ensuite la notification d’envoi sur cet appareil.</span><span class="sxs-lookup"><span data-stu-id="27eb6-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="27eb6-105">Voici les conditions préalables à l’appareil pour prendre en charge la réception de notifications personnalisées, et pour que l’application crée ensuite la notification d’envoi :</span><span class="sxs-lookup"><span data-stu-id="27eb6-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="27eb6-106">L’application portail d’entreprise doit être installée sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="27eb6-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="27eb6-107">L’appareil doit permettre à l’application portail d’entreprise d’envoyer des notifications de type émission.</span><span class="sxs-lookup"><span data-stu-id="27eb6-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="27eb6-108">Lorsque l’application est installée ou mise à jour, elle invite l’utilisateur à autoriser les notifications.</span><span class="sxs-lookup"><span data-stu-id="27eb6-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="27eb6-109">Google Play services doit être installé sur les appareils Android.</span><span class="sxs-lookup"><span data-stu-id="27eb6-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="27eb6-110">L’appareil doit être déployé avec Intune.</span><span class="sxs-lookup"><span data-stu-id="27eb6-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="27eb6-111">Pour plus d’informations sur l’envoi d’un message, consultez la documentation de la [fonctionnalité](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="27eb6-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
