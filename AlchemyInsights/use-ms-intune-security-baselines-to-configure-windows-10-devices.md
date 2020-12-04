---
title: Utiliser les bases de sécurité Microsoft Intune pour configurer les appareils Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571829"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utiliser les bases de sécurité Microsoft Intune pour configurer les appareils Windows 10

Les bases de sécurité Intune permettent de protéger les utilisateurs et les appareils. Les bases de sécurité sont des groupes préconfigurés des paramètres Windows utilisés pour appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité appropriées. En créant un profil de base de sécurité dans Intune, vous créez un modèle composé de plusieurs profils de configuration d’appareil.

Lorsque vous déployez des bases de sécurité vers des groupes d’utilisateurs ou de périphériques, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou version ultérieure. Par exemple, la ligne de base de sécurité MDM automatiquement (1) active BitLocker pour les lecteurs amovibles, (2) requiert le mot de passe pour déverrouiller un appareil, et (3) désactive l’authentification de base. Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, personnalisez la configuration de référence pour appliquer les paramètres dont vous avez besoin.

Les lignes de base de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365. Voici quelques avantages :

- Une base de sécurité inclut les meilleures pratiques et des recommandations pour les paramètres qui affectent la sécurité. Étant donné que les partenaires Intune avec l’équipe de sécurité Windows qui crée des configurations de référence pour les stratégies de groupe, ces recommandations sont basées sur des conseils solides et une grande expérience.
- Si vous débutez avec Intune et que vous n’êtes pas certain de l’emplacement de démarrage, les lignes de base de sécurité vous aideront à créer et déployer rapidement un profil sécurisé.
- Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune pour les besoins de la gestion est beaucoup plus facile avec les lignes de base de sécurité, car elles sont intégrées à Intune et incluent des fonctionnalités de pointe pour la gestion.

Pour en savoir plus, consultez la rubrique [Windows Security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).