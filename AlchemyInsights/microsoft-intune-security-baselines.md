---
title: Utiliser les Microsoft Intune de sécurité pour configurer Windows 10 appareils
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886630"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Utiliser les Microsoft Intune de sécurité pour configurer Windows 10 appareils

Les lignes de référence de sécurité d’Intune permettent de protéger les utilisateurs et les appareils. Les lignes de base de sécurité Windows des groupes pré-configurés utilisés pour appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité concernées. En créant un profil de ligne de référence de sécurité dans Intune, vous créez un modèle constitué de plusieurs profils de configuration des appareils.

Lorsque vous déployez des lignes de base de sécurité sur des groupes d’utilisateurs ou d’appareils, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou ultérieures. Par exemple, la ligne de base de sécurité de la gestion des périphériques mobiles (MDM) de Microsoft active automatiquement BitLocker pour les lecteurs amovibles, requiert le mot de passe pour déverrouiller un appareil et désactive l’authentification de base. Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, vous pouvez personnaliser la ligne de référence pour appliquer les paramètres dont vous avez besoin.

Les lignes de référence de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365. Une ligne de référence de sécurité inclut les meilleures pratiques et recommandations en matière de paramètres qui ont un impact sur la sécurité. Intune est partenaire de l’équipe de sécurité Windows qui crée des bases de référence pour les stratégies de groupe. Ces recommandations sont donc basées sur des conseils solide et une expérience étendue.

Si vous débutez avec Intune et que vous ne savez pas où commencer, les lignes de base de sécurité vous aident à créer et déployer rapidement un profil sécurisé. Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune à des fins de gestion est beaucoup plus facile avec les lignes de base de sécurité, car elles sont intégrées à Intune et incluent des fonctionnalités de gestion de pointe.

Pour en savoir plus, consultez [les Windows de sécurité](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) et la gestion des appareils [mobiles.](https://docs.microsoft.com/windows/client-management/mdm/)

