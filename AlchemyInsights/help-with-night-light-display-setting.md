---
title: Aide sur le paramètre d’affichage en mode clair de nuit
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123078"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="6df1e-102">Aide sur le paramètre d’affichage en mode clair de nuit</span><span class="sxs-lookup"><span data-stu-id="6df1e-102">Help with the night light display setting</span></span>

<span data-ttu-id="6df1e-103">Pour en savoir plus sur les paramètres d’affichage de nuit, consultez, [Définir l’affichage en mode nuit dans Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="6df1e-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="6df1e-104">Si les options du mode clair de nuit sont grisées dans les Paramètres, vérifiez votre pilote d’affichage :</span><span class="sxs-lookup"><span data-stu-id="6df1e-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="6df1e-105">Dans la zone de recherche de la barre des tâches, tapez **Gestionnaire d’appareil**, puis sélectionnez **Gestionnaire d’appareil** dans les résultats de la recherche.</span><span class="sxs-lookup"><span data-stu-id="6df1e-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="6df1e-106">Développez l’option **Afficher des adaptateurs**.</span><span class="sxs-lookup"><span data-stu-id="6df1e-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="6df1e-107">Malheureusement, la fonctionnalité du mode clair de nuit n’est pas disponible, si votre appareil utilise un pilote DisplayLink ou un pilote Affichage simple.</span><span class="sxs-lookup"><span data-stu-id="6df1e-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="6df1e-108">La fonctionnalité du mode clair de nuit utilise la technologie graphique récente. La mise à jour de votre pilote d’affichage pourrait donc être nécessaire :</span><span class="sxs-lookup"><span data-stu-id="6df1e-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="6df1e-109">Recherchez les mises à jour en accédant à **Démarrer** > **Paramètres** > **Mise à jour et sécurité** > **Windows Update** > **Vérifier les mises à jour**.</span><span class="sxs-lookup"><span data-stu-id="6df1e-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="6df1e-110">OU</span><span class="sxs-lookup"><span data-stu-id="6df1e-110">OR</span></span>

- <span data-ttu-id="6df1e-111">Visitez le site web du support de votre fabricant de matériel pour télécharger et installer manuellement les derniers pilotes d’affichage.</span><span class="sxs-lookup"><span data-stu-id="6df1e-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="6df1e-112">Réinitialiser le mode clair de nuit dans le registre</span><span class="sxs-lookup"><span data-stu-id="6df1e-112">Reset night light in the registry</span></span>

<span data-ttu-id="6df1e-113">Si la mise à jour de votre pilote d’affichage n’a pas fonctionné, vous devrez peut-être réinitialiser le mode clair de nuit dans le registre.</span><span class="sxs-lookup"><span data-stu-id="6df1e-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="6df1e-114">**Attention :** Cette étape de la résolution de problèmes est recommandée uniquement pour des utilisateurs avancés.</span><span class="sxs-lookup"><span data-stu-id="6df1e-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="6df1e-115">Des problèmes graves peuvent se produire si vous modifiez le registre de façon incorrecte.</span><span class="sxs-lookup"><span data-stu-id="6df1e-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="6df1e-116">Pour une protection supplémentaire, veuillez sauvegarder le registre avant de le modifier, afin de pouvoir le restaurer en cas de problème.</span><span class="sxs-lookup"><span data-stu-id="6df1e-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="6df1e-117">Dans la zone de recherche, tapez **Regedit**, puis sélectionnez **Éditeur de registre** dans les résultats de  recherche.</span><span class="sxs-lookup"><span data-stu-id="6df1e-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="6df1e-118">Accédez à cette clé de registre :</span><span class="sxs-lookup"><span data-stu-id="6df1e-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="6df1e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="6df1e-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="6df1e-120">Exportez, puis supprimez cette valeur subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="6df1e-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="6df1e-121">Exportez, puis supprimez cette valeur subkey:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="6df1e-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="6df1e-122">Redémarrez Windows et vérifiez si les options du mode clair de nuit sont disponibles.</span><span class="sxs-lookup"><span data-stu-id="6df1e-122">Restart Windows and verify if the night light options are available.</span></span>


