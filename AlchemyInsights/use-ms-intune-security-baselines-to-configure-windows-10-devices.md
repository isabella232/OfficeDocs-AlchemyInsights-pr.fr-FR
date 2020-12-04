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
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="f2bb1-102">Utiliser les bases de sécurité Microsoft Intune pour configurer les appareils Windows 10</span><span class="sxs-lookup"><span data-stu-id="f2bb1-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="f2bb1-103">Les bases de sécurité Intune permettent de protéger les utilisateurs et les appareils.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f2bb1-104">Les bases de sécurité sont des groupes préconfigurés des paramètres Windows utilisés pour appliquer un groupe connu de paramètres et de valeurs par défaut recommandés par les équipes de sécurité appropriées.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f2bb1-105">En créant un profil de base de sécurité dans Intune, vous créez un modèle composé de plusieurs profils de configuration d’appareil.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f2bb1-106">Lorsque vous déployez des bases de sécurité vers des groupes d’utilisateurs ou de périphériques, les paramètres sont appliqués aux appareils qui s’exécutent sur Windows 10 ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="f2bb1-107">Par exemple, la ligne de base de sécurité MDM automatiquement (1) active BitLocker pour les lecteurs amovibles, (2) requiert le mot de passe pour déverrouiller un appareil, et (3) désactive l’authentification de base.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="f2bb1-108">Lorsqu’une valeur par défaut ne fonctionne pas pour votre environnement, personnalisez la configuration de référence pour appliquer les paramètres dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f2bb1-109">Les lignes de base de sécurité permettent également d’établir un flux de travail sécurisé de bout en bout dans Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f2bb1-110">Voici quelques avantages :</span><span class="sxs-lookup"><span data-stu-id="f2bb1-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="f2bb1-111">Une base de sécurité inclut les meilleures pratiques et des recommandations pour les paramètres qui affectent la sécurité.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f2bb1-112">Étant donné que les partenaires Intune avec l’équipe de sécurité Windows qui crée des configurations de référence pour les stratégies de groupe, ces recommandations sont basées sur des conseils solides et une grande expérience.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="f2bb1-113">Si vous débutez avec Intune et que vous n’êtes pas certain de l’emplacement de démarrage, les lignes de base de sécurité vous aideront à créer et déployer rapidement un profil sécurisé.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="f2bb1-114">Si vous utilisez actuellement une stratégie de groupe, la migration vers Intune pour les besoins de la gestion est beaucoup plus facile avec les lignes de base de sécurité, car elles sont intégrées à Intune et incluent des fonctionnalités de pointe pour la gestion.</span><span class="sxs-lookup"><span data-stu-id="f2bb1-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="f2bb1-115">Pour en savoir plus, consultez la rubrique [Windows Security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile Device Management](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="f2bb1-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>