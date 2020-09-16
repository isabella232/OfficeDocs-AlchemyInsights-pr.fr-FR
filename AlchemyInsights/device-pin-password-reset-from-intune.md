---
title: Réinitialisation des mots de passe/code confidentiel de l’appareil à partir d'Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: 66255fc87a55161158aa4121d68d7ccd04b552ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730985"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="14947-102">Réinitialisation des mots de passe/code confidentiel de l’appareil à partir d'Intune</span><span class="sxs-lookup"><span data-stu-id="14947-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="14947-103">Vous pouvez supprimer un code secret ou forcer un utilisateur à créer un code secret dans Intune pour un appareil exécutant iOS ou Android à l’aide de l’action Supprimer le code secret.</span><span class="sxs-lookup"><span data-stu-id="14947-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="14947-104">Seuls les types de système d’exploitation et de profil professionnel spécifiques prennent en charge cette action.</span><span class="sxs-lookup"><span data-stu-id="14947-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="14947-105">Pour plus d’informations sur les plateformes prises en charge et le déclenchement de l’action de réinitialisation du code secret, consultez [Réinitialiser ou supprimer un code secret de l’appareil dans Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span><span class="sxs-lookup"><span data-stu-id="14947-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="14947-106">Vous pouvez réinitialiser un code confidentiel existant à l’aide de l’action de réinitialisation du code confidentiel sur les appareils exécutant le système d’exploitation Windows 10 mobile.</span><span class="sxs-lookup"><span data-stu-id="14947-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="14947-107">Cela permet à l’utilisateur de déverrouiller l’appareil et de créer un nouveau code confidentiel, le cas échéant.</span><span class="sxs-lookup"><span data-stu-id="14947-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="14947-108">Pour plus d’informations, consultez [Réinitialiser le code secret sur les appareils Windows à l’aide de Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span><span class="sxs-lookup"><span data-stu-id="14947-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>