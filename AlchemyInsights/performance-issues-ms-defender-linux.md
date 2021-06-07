---
title: Problèmes de performances pour Microsoft Defender pour point de terminaison sur Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783421"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="0c694-102">Problèmes de performances pour Microsoft Defender pour point de terminaison sur Linux</span><span class="sxs-lookup"><span data-stu-id="0c694-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="0c694-103">Cet article vous guide tout au long des étapes d’identification des problèmes de performances pour Microsoft Defender pour point de terminaison sur Linux.</span><span class="sxs-lookup"><span data-stu-id="0c694-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="0c694-104">Il est important de vérifier d’abord que le problème que vous rencontrez est résolu avec la [dernière version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="0c694-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="0c694-105">Pour démarrer votre investigation, consultez [Résoudre les problèmes de performances de Microsoft Defender pour point de terminaison sur Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="0c694-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="0c694-106">Exclusions</span><span class="sxs-lookup"><span data-stu-id="0c694-106">Exclusions</span></span>

<span data-ttu-id="0c694-107">Les exclusions peuvent aider à atténuer les problèmes de performances.</span><span class="sxs-lookup"><span data-stu-id="0c694-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="0c694-108">Passez en revue vos exclusions avant de commencer afin que tout risque supplémentaire soit connu et documenté.</span><span class="sxs-lookup"><span data-stu-id="0c694-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="0c694-109">Pour plus d’informations, consultez [Configurer et valider les exclusions pour Microsoft Defender pour point de terminaison sur Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="0c694-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="0c694-110">Lorsque vous avez plusieurs fichiers et dossiers à exclure et qu’ils sont tous sur le même point de montage, il peut être plus facile d’exclure le point de montage.</span><span class="sxs-lookup"><span data-stu-id="0c694-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="0c694-111">À compter de la version 101.22.80 de février, vous pouvez exclure un point de montage entier.</span><span class="sxs-lookup"><span data-stu-id="0c694-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="0c694-112">Par exemple, si /mnt/backup est un point de montage, vous pouvez ajouter /mnt/backup à la liste d’exclusion en exécutant cette commande :</span><span class="sxs-lookup"><span data-stu-id="0c694-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="0c694-113">**Remarque**: l’ajout d’exclusions augmente le risque que des programmes malveillants ne soient pas détectés et qu’ils doivent être gérés et implémentés avec précaution.</span><span class="sxs-lookup"><span data-stu-id="0c694-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="0c694-114">Besoin d’aide ?</span><span class="sxs-lookup"><span data-stu-id="0c694-114">Need Help?</span></span>

<span data-ttu-id="0c694-115">Pour vous aider de la manière la plus efficace possible, collectez les données de diagnostic avant d’ouvrir un cas de support.</span><span class="sxs-lookup"><span data-stu-id="0c694-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
