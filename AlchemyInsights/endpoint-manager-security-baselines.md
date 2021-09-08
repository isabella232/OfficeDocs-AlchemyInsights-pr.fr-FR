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
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923552"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager : base de référence de sécurité

Les bases de référence de sécurité sont des groupes préconfigurés de paramètres Windows qui vous permettent d’appliquer les paramètres de sécurité recommandés par les équipes de sécurité appropriées. Ces bases de référence peuvent être personnalisées pour fournir uniquement les paramètres et valeurs souhaités. Pour plus d’informations sur les bases de référence de sécurité, consultez [Utiliser des bases de référence de sécurité pour configurer des appareils Windows 10 dans Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Il existe actuellement des bases de référence pour ces produits :

- Paramètres de sécurité MDM Windows
- Sécurité Microsoft Defender pour point de terminaison
- Microsoft Edge

Chaque base de référence est mise à jour périodiquement et publiée dans des versions incrémentielles. Chaque version ajoute ou supprime des paramètres de la version précédente, pour s’assurer que la base de référence répond aux instructions actuelles. La console des bases de référence de sécurité dans Sécurité du point de terminaison permet de comparer les différentes versions en rendant visibles les modifications apportées d’une version à une autre.

Pour obtenir des instructions sur la modification efficace de la base de référence déployée, consultez [Gérer les profils d’une base de référence de sécurité dans Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Après avoir déployé une base de référence de sécurité, vous pouvez surveiller l’état du déploiement et passer en revue les paramètres de chaque appareil.

Étant donné que les lignes de base de sécurité contiennent de nombreux paramètres, il est important de passer en revue les modifications de configuration et d’effectuer des tests pour vous assurer que tous les paramètres sont appropriés pour vos appareils et vos besoins métiers.

**Remarque :** l’affichage du rapport des données de base de référence peut prendre jusqu’à 24 heures à partir du déploiement initial sur un appareil, et jusqu’à 6 heures pour des mises à jour supplémentaires. 

La raison la plus fréquente de l’inapplication d’un paramètre de base de référence, est l’utilisation du même paramètre dans un autre profil. Ce scénario peut être recherché pour un appareil spécifique en le sélectionnant dans le nœud État de l’appareil du profil de base de référence de sécurité. Pour plus d’informations, consultez [Résoudre des conflits de base de référence de sécurité](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).