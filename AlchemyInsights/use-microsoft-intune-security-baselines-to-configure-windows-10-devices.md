---
title: Utiliser les lignes de référence de sécurité Microsoft Intune pour configurer les appareils Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641619"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Utiliser les lignes de référence de sécurité Microsoft Intune pour la configuration des appareils Windows 10

Les lignes de référence de sécurité d’Intune permettent de protéger les utilisateurs et les appareils. Les lignes de référence de sécurité sont des groupes préconfigurés de paramètres Windows qui vous permettent d’appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité appropriées. En créant un profil de ligne de référence de sécurité dans Intune, vous créez un modèle constitué de plusieurs profils de configuration des appareils.

Lorsque vous déployez des lignes de référence de sécurité sur des groupes d’utilisateurs ou d’appareils, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou versions ultérieures. Par exemple, la ligne de référence de sécurité de la gestion des périphériques mobiles Microsoft (1) active automatiquement BitLocker pour les lecteurs amovibles, (2) requiert le mot de passe pour déverrouiller un appareil et (3) désactive l’authentification de base. Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, vous pouvez personnaliser la ligne de référence pour appliquer les paramètres dont vous avez besoin.

Les lignes de référence de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365. Voici quelques avantages de cette fonctionnalité :
- Une ligne de référence de sécurité inclut les meilleures pratiques et recommandations en matière de paramètres qui ont un impact sur la sécurité. Étant donné qu’Intune travaille en partenariat avec l’équipe de sécurité Windows ayant créé les lignes de référence des stratégies de groupe, ces recommandations sont basées sur des instructions solides et une expérience étendue.
- Si vous débutez avec Intune et que vous ne savez pas où commencer, les lignes de référence de sécurité vous aideront à créer et à déployer rapidement un profil sécurisé.
- Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune à des fins de gestion est beaucoup plus simple avec les lignes de référence de sécurité, car ces lignes de référence de sécurité sont intégrées dans Intune et incluent des fonctionnalités de pointe de la gestion.

Pour plus d’informations, consultez [Ligne de référence de sécurité Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) et [Gestion d’un appareil mobile](https://docs.microsoft.com/windows/client-management/mdm/).