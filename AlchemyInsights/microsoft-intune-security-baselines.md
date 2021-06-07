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
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783190"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="602a0-102">Utiliser les Microsoft Intune de sécurité pour configurer Windows 10 appareils</span><span class="sxs-lookup"><span data-stu-id="602a0-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="602a0-103">Les lignes de référence de sécurité d’Intune permettent de protéger les utilisateurs et les appareils.</span><span class="sxs-lookup"><span data-stu-id="602a0-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="602a0-104">Les lignes de base de sécurité Windows des groupes pré-configurés utilisés pour appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité concernées.</span><span class="sxs-lookup"><span data-stu-id="602a0-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="602a0-105">En créant un profil de ligne de référence de sécurité dans Intune, vous créez un modèle constitué de plusieurs profils de configuration des appareils.</span><span class="sxs-lookup"><span data-stu-id="602a0-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="602a0-106">Lorsque vous déployez des lignes de base de sécurité sur des groupes d’utilisateurs ou d’appareils, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou ultérieures.</span><span class="sxs-lookup"><span data-stu-id="602a0-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="602a0-107">Par exemple, la ligne de base de sécurité de la gestion des périphériques mobiles (MDM) de Microsoft active automatiquement BitLocker pour les lecteurs amovibles, requiert le mot de passe pour déverrouiller un appareil et désactive l’authentification de base.</span><span class="sxs-lookup"><span data-stu-id="602a0-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="602a0-108">Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, vous pouvez personnaliser la ligne de référence pour appliquer les paramètres dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="602a0-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="602a0-109">Les lignes de référence de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="602a0-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="602a0-110">Une ligne de référence de sécurité inclut les meilleures pratiques et recommandations en matière de paramètres qui ont un impact sur la sécurité.</span><span class="sxs-lookup"><span data-stu-id="602a0-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="602a0-111">Intune est partenaire de l’équipe de sécurité Windows qui crée des bases de référence pour les stratégies de groupe. Ces recommandations sont donc basées sur des conseils solide et une expérience étendue.</span><span class="sxs-lookup"><span data-stu-id="602a0-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="602a0-112">Si vous débutez avec Intune et que vous ne savez pas où commencer, les lignes de base de sécurité vous aident à créer et déployer rapidement un profil sécurisé.</span><span class="sxs-lookup"><span data-stu-id="602a0-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="602a0-113">Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune à des fins de gestion est beaucoup plus facile avec les lignes de base de sécurité, car elles sont intégrées à Intune et incluent des fonctionnalités de gestion de pointe.</span><span class="sxs-lookup"><span data-stu-id="602a0-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="602a0-114">Pour en savoir plus, consultez [les Windows de sécurité](/windows/security/threat-protection/windows-security-baselines) et la gestion des appareils [mobiles.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="602a0-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

