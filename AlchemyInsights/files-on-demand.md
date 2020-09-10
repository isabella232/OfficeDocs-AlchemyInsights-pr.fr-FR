---
title: Fichiers à la demande
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406562"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="69c38-102">Configurer les fichiers à la demande</span><span class="sxs-lookup"><span data-stu-id="69c38-102">Configure Files On-Demand</span></span>

<span data-ttu-id="69c38-103">La fonctionnalité Fichiers à la demande OneDrive vous permet d’accéder à vos fichiers dans OneDrive sans avoir à en télécharger la totalité et à utiliser l’espace de stockage de votre appareil.</span><span class="sxs-lookup"><span data-stu-id="69c38-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="69c38-104">Pour configurer les fichiers à la demande sur votre PC :</span><span class="sxs-lookup"><span data-stu-id="69c38-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="69c38-105">Sélectionnez l’icône de nuage **OneDrive** blanc ou bleu dans la zone de notification de la barre des tâches Windows.</span><span class="sxs-lookup"><span data-stu-id="69c38-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="69c38-106">Sélectionnez l'icône d’engrenages **Aide & paramètres** > **Paramètres**.</span><span class="sxs-lookup"><span data-stu-id="69c38-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="69c38-107">Dans l’onglet **Paramètres**, cochez la case **Libérez de l’espace et téléchargez des fichiers lorsque vous avez besoin de les utiliser**.</span><span class="sxs-lookup"><span data-stu-id="69c38-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="69c38-108">Vous pouvez également configurer les fichiers à la demande à l’aide du registre.</span><span class="sxs-lookup"><span data-stu-id="69c38-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="69c38-109">Si vous désactivez ce paramètre, les utilisateurs de Windows 10 ont le même comportement de synchronisation que les utilisateurs des versions précédentes de Windows et ne peuvent pas activer la fonctionnalité Fichiers à la demande.</span><span class="sxs-lookup"><span data-stu-id="69c38-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="69c38-110">Si vous ne configurez pas ce paramètre, les utilisateurs peuvent activer la fonctionnalité Fichiers à la demande ou la désactiver.</span><span class="sxs-lookup"><span data-stu-id="69c38-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="69c38-111">Cette stratégie définit la valeur de la clé de Registre suivante sur 1.</span><span class="sxs-lookup"><span data-stu-id="69c38-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="69c38-112">Désactiver cette stratégie définit la valeur de la clé de registre suivante sur 0.</span><span class="sxs-lookup"><span data-stu-id="69c38-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="69c38-113">Si vous l’option Fichiers à la demande n’apparaît pas dans l’onglet Paramètres, assurez-vous que le type de démarrage du service Pilote de filtrage de fichiers dans le cloud Windows est défini sur 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="69c38-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="69c38-114">Activer cette fonctionnalité définit la valeur de la clé de registre suivante sur 2.</span><span class="sxs-lookup"><span data-stu-id="69c38-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`