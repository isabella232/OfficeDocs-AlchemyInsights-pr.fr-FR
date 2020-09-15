---
title: Suppression des données et réinitialisation d’appareils dans Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701281"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="92327-102">Suppression des données et réinitialisation d’appareils dans Intune</span><span class="sxs-lookup"><span data-stu-id="92327-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="92327-103">Les actions à distance Mise hors service et Réinitialisation peuvent être utilisées pour supprimer les données de l'entreprise gérées par Intune ou pour effectuer une réinitialisation aux paramètres d'usine et rétablir les paramètres par défaut de l'appareil.</span><span class="sxs-lookup"><span data-stu-id="92327-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="92327-104">Connectez-vous à la gestion des appareils Microsoft 365 et accédez à **Appareils** > **Tous les appareils**.</span><span class="sxs-lookup"><span data-stu-id="92327-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="92327-105">Sélectionnez l’appareil que vous voulez réinitialiser.</span><span class="sxs-lookup"><span data-stu-id="92327-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="92327-106">Sélectionnez le type de réinitialisation à distance que vous voulez effectuer.</span><span class="sxs-lookup"><span data-stu-id="92327-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="92327-107">La mise hors service supprime uniquement les informations de l’organisation, tandis que les réinitialisations complètes restaurent les paramètres par défaut de l’appareil.</span><span class="sxs-lookup"><span data-stu-id="92327-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="92327-108">Cliquez sur **Oui** pour confirmer.</span><span class="sxs-lookup"><span data-stu-id="92327-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="92327-109">Jusqu’à la fin de la réinitialisation, l’état d’action de l’appareil indique comme Mise hors service en attente.</span><span class="sxs-lookup"><span data-stu-id="92327-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="92327-110">Une fois l’action terminée, vous ne verrez plus l’appareil mobile dans la liste des appareils gérés.</span><span class="sxs-lookup"><span data-stu-id="92327-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="92327-111">**Remarque** les données de l’entreprise ne peuvent pas être supprimées des appareils joints à Azure AD.</span><span class="sxs-lookup"><span data-stu-id="92327-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="92327-112">Pour plus d’informations sur l’effet des actions de Mise hors service et Réinitialisation, notamment les éléments conservés et les éléments supprimés, consultez [Supprimer des appareils à l’aide de l’opération de réinitialisation, de mise hors service ou de désinscription manuelle de l’appareil](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="92327-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="92327-113">Pour effacer toutes les données d’un appareil macOS, consultez [Effacer toutes les données d’un appareil macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="92327-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>