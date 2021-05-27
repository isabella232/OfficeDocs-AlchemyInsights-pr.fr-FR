---
title: Règles de réduction des surfaces d'attaque
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651485"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="3342d-102">Règles de réduction des surfaces d'attaque</span><span class="sxs-lookup"><span data-stu-id="3342d-102">Attack surface reduction rules</span></span>

<span data-ttu-id="3342d-103">L’exclusion des fichiers ou dossiers peut considérablement réduire la protection fournie par les règles de réduction de la surface d’attaque.</span><span class="sxs-lookup"><span data-stu-id="3342d-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="3342d-104">Les fichiers qui auraient été bloqués par une règle sont autorisés à s’exécuter, et aucun rapport ou événement n’est enregistré.</span><span class="sxs-lookup"><span data-stu-id="3342d-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="3342d-105">Une exclusion s’applique à toutes les règles qui autorisent les exclusions.</span><span class="sxs-lookup"><span data-stu-id="3342d-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="3342d-106">Les exclusions ASR utilisent la même syntaxe que les exclusions de l’Antivirus Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="3342d-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="3342d-107">Pour plus d’informations, consultez [Configurer et valider les exclusions pour les analyse Antivirus Microsoft Defender](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="3342d-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="3342d-108">Pour éviter des problèmes, passez en revue [Erreurs courantes à éviter lors de la définition d’exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="3342d-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="3342d-109">Toutes les règles de réduction de la surface d’attaque ne prennent pas en charge les exclusions.</span><span class="sxs-lookup"><span data-stu-id="3342d-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="3342d-110">Pour vérifier si votre règle prend en charge les exclusions, consultez le tableau [Règles de réduction de la surface d’attaque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="3342d-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="3342d-111">Règles de réduction des surfaces d'attaque</span><span class="sxs-lookup"><span data-stu-id="3342d-111">Attack surface reduction rules</span></span>

<span data-ttu-id="3342d-112">La surface d'attaque de votre organisation comprend tous les endroits où un attaquant pourrait compromettre les appareils ou les réseaux de l'organisation.</span><span class="sxs-lookup"><span data-stu-id="3342d-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="3342d-113">Réduire votre surface d’attaque implique de protéger les appareils et le réseau de l’organisation, ce qui laisse aux attaquants moins de moyens d’effectuer des attaques.</span><span class="sxs-lookup"><span data-stu-id="3342d-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="3342d-114">La configuration des règles de réduction des surface d’attaque dans Microsoft Defender pour point de terminaison peut vous aider.</span><span class="sxs-lookup"><span data-stu-id="3342d-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="3342d-115">Pour plus d'informations, voir :</span><span class="sxs-lookup"><span data-stu-id="3342d-115">For more information, see:</span></span>

- [<span data-ttu-id="3342d-116">Guid de la règle de réduction de la surface d’attaque de carte vers le nom</span><span class="sxs-lookup"><span data-stu-id="3342d-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="3342d-117">Règles de réduction de la surface d’attaque requises :</span><span class="sxs-lookup"><span data-stu-id="3342d-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="3342d-118">Windows 10 Professionnel, version 1709 ou ultérieure</span><span class="sxs-lookup"><span data-stu-id="3342d-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="3342d-119">Windows 10 Entreprise, version 1709 ou ultérieure</span><span class="sxs-lookup"><span data-stu-id="3342d-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="3342d-120">Windows Server, version 1803 (Canal semi-annuel) ou ultérieure</span><span class="sxs-lookup"><span data-stu-id="3342d-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="3342d-121">Identifier l’exclusion correcte à appliquer</span><span class="sxs-lookup"><span data-stu-id="3342d-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="3342d-122">Recherchez eventID 1121 ou 1122 dans le journal opérationnel/Microsoft-Windows-Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="3342d-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="3342d-123">Évaluez le scénario de blocage et le contexte et confirmez que ce scénario doit être débloqué.</span><span class="sxs-lookup"><span data-stu-id="3342d-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="3342d-124">Lisez la valeur Path dans les détails de l'événement, qui est la valeur qui définit l'exclusion.</span><span class="sxs-lookup"><span data-stu-id="3342d-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="3342d-125">Rendez l’exclusion aussi stricte que possible.</span><span class="sxs-lookup"><span data-stu-id="3342d-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="3342d-126">Appliquez un caractère générique si nécessaire (par exemple, remplacer la variable Utilisateur).</span><span class="sxs-lookup"><span data-stu-id="3342d-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="3342d-127">Appliquez l’exclusion en fonction de vos besoins de déploiement.</span><span class="sxs-lookup"><span data-stu-id="3342d-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="3342d-128">Pour plus d’informations, consultez [Personnaliser les règles de réduction de la surface d’attaque](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="3342d-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="3342d-129">L’exclusion n’est pas respectée</span><span class="sxs-lookup"><span data-stu-id="3342d-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="3342d-130">Déterminez si la règle prend en charge les exclusions.</span><span class="sxs-lookup"><span data-stu-id="3342d-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="3342d-131">Pour plus d’informations, consultez [Règles de réduction de la surface d’attaque](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="3342d-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="3342d-132">Passez en revue les exclusions appliquées et vérifiez avec les données d’événement les fautes de frappe ou les caractères génériques mal interprétés.</span><span class="sxs-lookup"><span data-stu-id="3342d-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="3342d-133">Pour plus d’informations, consultez [Types d’exclusion pris en charge](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="3342d-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="3342d-134">si l'impact de la règle est trop élevé, envisagez de faire passer la règle (de nouveau) en mode Audit pour effectuer une validation supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="3342d-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="3342d-135">Pour plus d’informations, consultez [Tester le fonctionnement des fonctionnalités de Microsoft Defender pour point de terminaison en mode Audit](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="3342d-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="3342d-136">Collectez les données de support pour ouvrir un cas de support à l’aide de cette commande :</span><span class="sxs-lookup"><span data-stu-id="3342d-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="3342d-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="3342d-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="3342d-138">Pour plus d’informations, consultez [Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="3342d-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
