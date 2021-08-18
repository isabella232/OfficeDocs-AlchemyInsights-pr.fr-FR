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
ms.openlocfilehash: b1200f0dd206e27cccf96778beb0326c846e7504e51be283193b2630edfb4509
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086738"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problèmes de performances pour Microsoft Defender pour point de terminaison sur Linux

Cet article vous guide tout au long des étapes d’identification des problèmes de performances pour Microsoft Defender pour point de terminaison sur Linux.

Il est important de vérifier d’abord que le problème que vous rencontrez est résolu avec la [dernière version](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

Pour démarrer votre investigation, consultez [Résoudre les problèmes de performances de Microsoft Defender pour point de terminaison sur Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Exclusions

Les exclusions peuvent aider à atténuer les problèmes de performances. Passez en revue vos exclusions avant de commencer afin que tout risque supplémentaire soit connu et documenté.

Pour plus d’informations, consultez [Configurer et valider les exclusions pour Microsoft Defender pour point de terminaison sur Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

Lorsque vous avez plusieurs fichiers et dossiers à exclure et qu’ils sont tous sur le même point de montage, il peut être plus facile d’exclure le point de montage. À compter de la version 101.22.80 de février, vous pouvez exclure un point de montage entier.

Par exemple, si /mnt/backup est un point de montage, vous pouvez ajouter /mnt/backup à la liste d’exclusion en exécutant cette commande :

`$ mdatp exclusion folder add –path /mnt/backup`

**Remarque**: l’ajout d’exclusions augmente le risque que des programmes malveillants ne soient pas détectés et qu’ils doivent être gérés et implémentés avec précaution.

## <a name="need-help"></a>Besoin d’aide ?

Pour vous aider de la manière la plus efficace possible, collectez les données de diagnostic avant d’ouvrir un cas de support.
