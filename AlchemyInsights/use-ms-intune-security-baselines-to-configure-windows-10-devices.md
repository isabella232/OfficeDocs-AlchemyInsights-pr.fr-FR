---
title: Utiliser les Microsoft Intune de sécurité pour configurer Windows 10 appareils
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104342"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utiliser les Microsoft Intune de sécurité pour configurer Windows 10 appareils

Les lignes de référence de sécurité d’Intune permettent de protéger les utilisateurs et les appareils. Les lignes de référence de sécurité sont des groupes préconfigurés de paramètres Windows qui vous permettent d’appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité appropriées. En créant un profil de ligne de référence de sécurité dans Intune, vous créez un modèle constitué de plusieurs profils de configuration des appareils.

Lorsque vous déployez des lignes de base de sécurité sur des groupes d’utilisateurs ou d’appareils, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou ultérieures. Par exemple, la ligne de base de sécurité MDM active automatiquement (1) BitLocker pour les lecteurs amovibles, (2) requiert le mot de passe pour déverrouiller un appareil et (3) désactive l’authentification de base. Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, personnalisez la ligne de base pour appliquer les paramètres dont vous avez besoin.

Les lignes de référence de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365. Voici quelques-uns des avantages suivants :

- Une ligne de référence de sécurité inclut les meilleures pratiques et recommandations en matière de paramètres qui ont un impact sur la sécurité. Étant donné qu’Intune travaille en partenariat avec l’équipe de sécurité Windows ayant créé les lignes de référence des stratégies de groupe, ces recommandations sont basées sur des instructions solides et une expérience étendue.
- Si vous débutez avec Intune et que vous ne savez pas où commencer, les lignes de référence de sécurité vous aideront à créer et à déployer rapidement un profil sécurisé.
- Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune à des fins de gestion est beaucoup plus facile avec les lignes de base de sécurité, car elles sont intégrées à Intune et incluent des fonctionnalités de pointe pour la gestion.

Pour en savoir plus, [consultez les Windows de sécurité](https://go.microsoft.com/fwlink/?linkid=2141503) et la gestion des appareils [mobiles.](https://go.microsoft.com/fwlink/?linkid=2141701)