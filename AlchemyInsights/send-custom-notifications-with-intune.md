---
title: Envoyer des notifications personnalisées avec Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886855"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="aa1c2-102">Comment envoyer des notifications personnalisées aux utilisateurs des appareils iOS et Android gérés</span><span class="sxs-lookup"><span data-stu-id="aa1c2-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="aa1c2-103">Les notifications personnalisées pour Intune sont traitées par l’application portail d’entreprise sur l’appareil d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="aa1c2-104">L’application crée ensuite la notification d’envoi sur cet appareil.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="aa1c2-105">Voici les conditions préalables à l’appareil pour prendre en charge la réception de notifications personnalisées, et pour que l’application crée ensuite la notification d’envoi :</span><span class="sxs-lookup"><span data-stu-id="aa1c2-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="aa1c2-106">L’application portail d’entreprise doit être installée sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="aa1c2-107">L’appareil doit permettre à l’application portail d’entreprise d’envoyer des notifications de type émission.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="aa1c2-108">Lorsque l’application est installée ou mise à jour, elle invite l’utilisateur à autoriser les notifications.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="aa1c2-109">Google Play services doit être installé sur les appareils Android.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="aa1c2-110">L’appareil doit être déployé avec Intune.</span><span class="sxs-lookup"><span data-stu-id="aa1c2-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="aa1c2-111">Pour plus d’informations sur l’envoi d’un message, consultez la documentation de la [fonctionnalité](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="aa1c2-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
