---
title: Enregistrement d’appareil dupliqué dans le portail
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678502"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="8899b-102">Enregistrement d’appareil dupliqué dans le portail</span><span class="sxs-lookup"><span data-stu-id="8899b-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="8899b-103">Vous pouvez voir 2 enregistrements pour un appareil dans le portail si l’appareil ne signale pas correctement l’état de la co-gestion sur le site de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8899b-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="8899b-104">Pour vérifier l’état de co-gestion d’un appareil, consultez la colonne **co-géré** de l’appareil dans la console de Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="8899b-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="8899b-105">Si la colonne n’est pas visible, vous pouvez l’ajouter en cliquant avec le bouton droit sur l’un des en-têtes de colonne, puis en sélectionnant celle-ci dans la liste.</span><span class="sxs-lookup"><span data-stu-id="8899b-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="8899b-106">La valeur Co-géré doit être définie sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="8899b-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="8899b-107">Si la valeur est définie sur **Non**, ouvrez l’applet client Configuration Manager sur l’appareil client et vérifiez la propriété **Co-gestion** dans l’onglet général.</span><span class="sxs-lookup"><span data-stu-id="8899b-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="8899b-108">Si la valeur est définie sur **Activé**, cela indique la présence de problèmes liés aux communications client avec le point de gestion.</span><span class="sxs-lookup"><span data-stu-id="8899b-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="8899b-109">Consultez le **CcmMessaging.log** sur l’appareil pour identifier les problèmes de connectivité potentiels.</span><span class="sxs-lookup"><span data-stu-id="8899b-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="8899b-110">Si la valeur est définit sur **désactivée** et si l’appareil est inscrit dans Intune, vérifiez que l’appareil a reçu la stratégie de co-gestion en examinant le **CoManagementHandler.log** sur l’appareil.</span><span class="sxs-lookup"><span data-stu-id="8899b-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
