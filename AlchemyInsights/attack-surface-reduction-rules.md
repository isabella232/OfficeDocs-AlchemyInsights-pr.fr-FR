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
ms.openlocfilehash: f7811c15af21d8e7790e6686bb8ba9e5de3659d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318994"
---
# <a name="attack-surface-reduction-rules"></a>Règles de réduction des surfaces d'attaque

L’exclusion des fichiers ou dossiers peut considérablement réduire la protection fournie par les règles de réduction de la surface d’attaque. Les fichiers qui auraient été bloqués par une règle sont autorisés à s’exécuter, et aucun rapport ou événement n’est enregistré. Une exclusion s’applique à toutes les règles qui autorisent les exclusions.

Les exclusions ASR utilisent la même syntaxe que les exclusions de l’Antivirus Microsoft Defender. Pour plus d’informations, consultez [Configurer et valider les exclusions pour les analyse Antivirus Microsoft Defender](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). Pour éviter des problèmes, passez en revue [Erreurs courantes à éviter lors de la définition d’exclusions](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Toutes les règles de réduction de la surface d’attaque ne prennent pas en charge les exclusions. Pour vérifier si votre règle prend en charge les exclusions, consultez le tableau [Règles de réduction de la surface d’attaque](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Règles de réduction des surfaces d'attaque

La surface d'attaque de votre organisation comprend tous les endroits où un attaquant pourrait compromettre les appareils ou les réseaux de l'organisation. Réduire votre surface d’attaque implique de protéger les appareils et le réseau de l’organisation, ce qui laisse aux attaquants moins de moyens d’effectuer des attaques. La configuration des règles de réduction des surface d’attaque dans Microsoft Defender pour point de terminaison peut vous aider.

Pour plus d'informations, voir :

- [Guid de la règle de réduction de la surface d’attaque de carte vers le nom](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Règles de réduction de la surface d’attaque requises :
    - [Windows 10 Professionnel, version 1709 ou ultérieure](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Entreprise, version 1709 ou ultérieure](https://docs.microsoft.com/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, version 1803 (Canal semi-annuel) ou ultérieure](https://docs.microsoft.com/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifier l’exclusion correcte à appliquer

1. Recherchez eventID 1121 ou 1122 dans le journal opérationnel/Microsoft-Windows-Windows Defender.

1. Évaluez le scénario de blocage et le contexte et confirmez que ce scénario doit être débloqué.

1. Lisez la valeur Path dans les détails de l'événement, qui est la valeur qui définit l'exclusion.
    - Rendez l’exclusion aussi stricte que possible.
    - Appliquez un caractère générique si nécessaire (par exemple, remplacer la variable Utilisateur).

1. Appliquez l’exclusion en fonction de vos besoins de déploiement. Pour plus d’informations, consultez [Personnaliser les règles de réduction de la surface d’attaque](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>L’exclusion n’est pas respectée

1. Déterminez si la règle prend en charge les exclusions. Pour plus d’informations, consultez [Règles de réduction de la surface d’attaque](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Passez en revue les exclusions appliquées et vérifiez avec les données d’événement les fautes de frappe ou les caractères génériques mal interprétés. Pour plus d’informations, consultez [Types d’exclusion pris en charge](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. si l'impact de la règle est trop élevé, envisagez de faire passer la règle (de nouveau) en mode Audit pour effectuer une validation supplémentaire. Pour plus d’informations, consultez [Tester le fonctionnement des fonctionnalités de Microsoft Defender pour point de terminaison en mode Audit](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/audit-windows-defender).

1. Collectez les données de support pour ouvrir un cas de support à l’aide de cette commande :
    
   ** MDEClientAnalyzer.cmd -v**

    Pour plus d’informations, consultez [Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison](issues-with-onboarding-machines.md).
