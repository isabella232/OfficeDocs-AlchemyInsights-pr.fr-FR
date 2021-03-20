---
title: Empêcher l’utilisateur d’enregistrer des réunions
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897674"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="ffa69-102">Empêcher l’utilisateur d’enregistrer des réunions</span><span class="sxs-lookup"><span data-stu-id="ffa69-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="ffa69-103">Si vous devez empêcher ou **empêcher** des utilisateurs spécifiques d’enregistrer des réunions Teams, vous pouvez le faire via les paramètres de stratégie de réunion Teams.</span><span class="sxs-lookup"><span data-stu-id="ffa69-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="ffa69-104">Dans le Centre d’administration Microsoft Teams, désactiver le paramètre Autoriser l’enregistrement **dans le cloud** dans la stratégie de réunion attribuée à cet utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ffa69-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="ffa69-105">Pour plus d’informations, voir [Gérer les stratégies de réunion dans Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="ffa69-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="ffa69-106">Pour vérifier si un utilisateur spécifique est autorisé ou non à enregistrer des réunions Teams, utilisez le diagnostic de support.</span><span class="sxs-lookup"><span data-stu-id="ffa69-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="ffa69-107">Exécutez une nouvelle requête de support et tapez **diag : enregistrement** de réunion : le diagnostic vérifie les paramètres de stratégie pour l’utilisateur spécifié et détermine ses paramètres de stratégie.</span><span class="sxs-lookup"><span data-stu-id="ffa69-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="ffa69-108">N’oubliez pas que l’application des nouveaux paramètres de stratégie peut prendre quelques heures. Par exemple, si vous avez apporté une modification, patientez quelques heures avant de recommencer le diagnostic.</span><span class="sxs-lookup"><span data-stu-id="ffa69-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="ffa69-109">Pour plus d’informations, [examinez Activer ou désactiver l’enregistrement dans le cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="ffa69-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
