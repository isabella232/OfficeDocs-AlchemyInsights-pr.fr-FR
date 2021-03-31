---
title: 'Endpoint Manager : base de référence de sécurité'
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440882"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="2da5d-102">Endpoint Manager : base de référence de sécurité</span><span class="sxs-lookup"><span data-stu-id="2da5d-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="2da5d-103">Les bases de référence de sécurité sont des groupes préconfigurés de paramètres Windows qui vous permettent d’appliquer les paramètres de sécurité recommandés par les équipes de sécurité appropriées.</span><span class="sxs-lookup"><span data-stu-id="2da5d-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="2da5d-104">Ces bases de référence peuvent être personnalisées pour fournir uniquement les paramètres et valeurs souhaités.</span><span class="sxs-lookup"><span data-stu-id="2da5d-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="2da5d-105">Pour plus d’informations sur les bases de référence de sécurité, consultez [Utiliser des bases de référence de sécurité pour configurer des appareils Windows 10 dans Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2da5d-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="2da5d-106">Il existe actuellement des bases de référence pour ces produits :</span><span class="sxs-lookup"><span data-stu-id="2da5d-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="2da5d-107">Paramètres de sécurité MDM Windows</span><span class="sxs-lookup"><span data-stu-id="2da5d-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="2da5d-108">Sécurité Microsoft Defender pour point de terminaison</span><span class="sxs-lookup"><span data-stu-id="2da5d-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="2da5d-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2da5d-109">Microsoft Edge</span></span>

<span data-ttu-id="2da5d-110">Chaque base de référence est mise à jour périodiquement et publiée dans des versions incrémentielles.</span><span class="sxs-lookup"><span data-stu-id="2da5d-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="2da5d-111">Chaque version ajoute ou supprime des paramètres de la version précédente, pour s’assurer que la base de référence répond aux instructions actuelles.</span><span class="sxs-lookup"><span data-stu-id="2da5d-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="2da5d-112">La console des bases de référence de sécurité dans Sécurité du point de terminaison permet de comparer les différentes versions en rendant visibles les modifications apportées d’une version à une autre.</span><span class="sxs-lookup"><span data-stu-id="2da5d-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="2da5d-113">Pour obtenir des instructions sur la modification efficace de la base de référence déployée, consultez [Gérer les profils d’une base de référence de sécurité dans Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="2da5d-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="2da5d-114">Après avoir déployé une base de référence de sécurité, vous pouvez surveiller l’état du déploiement et passer en revue les paramètres de chaque appareil.</span><span class="sxs-lookup"><span data-stu-id="2da5d-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="2da5d-115">**Remarque :** l’affichage du rapport des données de base de référence peut prendre jusqu’à 24 heures à partir du déploiement initial sur un appareil, et jusqu’à 6 heures pour des mises à jour supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="2da5d-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="2da5d-116">La raison la plus fréquente de l’inapplication d’un paramètre de base de référence, est l’utilisation du même paramètre dans un autre profil.</span><span class="sxs-lookup"><span data-stu-id="2da5d-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="2da5d-117">Ce scénario peut être recherché pour un appareil spécifique en le sélectionnant dans le nœud État de l’appareil du profil de base de référence de sécurité.</span><span class="sxs-lookup"><span data-stu-id="2da5d-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="2da5d-118">Pour plus d’informations, consultez [Résoudre des conflits de base de référence de sécurité](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="2da5d-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>