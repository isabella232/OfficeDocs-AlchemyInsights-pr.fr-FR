---
title: Nettoyage automatique des appareils obsolètes dans Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505187"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="af7d8-102">Nettoyage automatique des appareils obsolètes dans Intune</span><span class="sxs-lookup"><span data-stu-id="af7d8-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="af7d8-103">Intune permet à l’administrateur de configurer un intervalle de temps compris entre 90 et 270 jours, après quoi les appareils obsolètes sont supprimés du service.</span><span class="sxs-lookup"><span data-stu-id="af7d8-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="af7d8-104">Ce paramètre s’applique à l’échelle de l’organisation et une fois activés immédiatement.</span><span class="sxs-lookup"><span data-stu-id="af7d8-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="af7d8-105">Les appareils non archivés dans le serveur Intune pendant une période supérieure au paramètre sont supprimés définitivement.</span><span class="sxs-lookup"><span data-stu-id="af7d8-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="af7d8-106">**Remarque** seuls les objets appareil de la gestion des appareils mobiles sont éligibles pour cette action de nettoyage.</span><span class="sxs-lookup"><span data-stu-id="af7d8-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="af7d8-107">Seuls les objets de l'appareil EAS sont exclus.</span><span class="sxs-lookup"><span data-stu-id="af7d8-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="af7d8-108">Pour plus d’informations sur la suppression d’un appareil sur la base du paramètre de nettoyage de l’appareil et de son « état », procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="af7d8-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="af7d8-109">Paramètre : **supprimer les appareils après la dernière date d’archivage : Oui (valeur (N) dans jours spécifiés)**</span><span class="sxs-lookup"><span data-stu-id="af7d8-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="af7d8-110">En fonction de la valeur (N) configurée dans le paramètre, le service Intune supprime l’appareil dans les jours spécifiés après son dernier enregistrement réussi.</span><span class="sxs-lookup"><span data-stu-id="af7d8-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="af7d8-111">Paramètre : **supprimer les appareils après la dernière date d’archivage : non**</span><span class="sxs-lookup"><span data-stu-id="af7d8-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="af7d8-112">180 jours après l'expiration et le non-renouvellement du certificat de l'appareil, celui-ci est supprimé.</span><span class="sxs-lookup"><span data-stu-id="af7d8-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="af7d8-113">**Remarque** dans les deux cas, l’appareil doit être correctement inscrit dans Intune.</span><span class="sxs-lookup"><span data-stu-id="af7d8-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="af7d8-114">L’inscription a lieu pendant la première intégration de l’appareil avec le service Intune.</span><span class="sxs-lookup"><span data-stu-id="af7d8-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="af7d8-115">Si un appareil se met en relation avec Intune, mais qu’il n’a pas été inscrits dans Intune, l’appareil est supprimé 270 jours après l’inscription.</span><span class="sxs-lookup"><span data-stu-id="af7d8-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="af7d8-116">(90 jours pour marquer l’appareil comme révoqué, puis un autre 180 jours pour supprimer l’enregistrement.)</span><span class="sxs-lookup"><span data-stu-id="af7d8-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="af7d8-117">Il n’existe actuellement aucun mécanisme dans la console Intune pour définir la date d’expiration de la certification des appareils pour un appareil donné.</span><span class="sxs-lookup"><span data-stu-id="af7d8-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>