---
title: Ajouter Microsoft Edge à Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177991"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="a281e-102">Ajouter Microsoft Edge à Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a281e-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="a281e-103">Pour déployer, configurer, surveiller et protéger Microsoft Edge pour Windows 10, vous devez d’abord l’ajouter à Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a281e-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="a281e-104">Intune prend en charge Microsoft Edge 77 et versions ultérieures.</span><span class="sxs-lookup"><span data-stu-id="a281e-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="a281e-105">Intune détecte les installations pré-existantes de Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a281e-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="a281e-106">Si Microsoft Edge est installé dans le contexte de l’utilisateur, une installation système a pour effet de remplacer l’installation dans le contexte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a281e-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="a281e-107">Si Microsoft Edge est installé dans le contexte système, le succès de l’installation est signalé.</span><span class="sxs-lookup"><span data-stu-id="a281e-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="a281e-108">Les versions préinstallées de Microsoft Edge 77 et des versions ultérieures, pour tous les canaux dans le contexte utilisateur, seront remplacés par Microsoft Edge installé dans le contexte système.</span><span class="sxs-lookup"><span data-stu-id="a281e-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="a281e-109">**Conditions préalables**</span><span class="sxs-lookup"><span data-stu-id="a281e-109">**Prerequisite**</span></span>

<span data-ttu-id="a281e-110">Windows 10 version 1709 ou ultérieure</span><span class="sxs-lookup"><span data-stu-id="a281e-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="a281e-111">**Étapes d’ajout de Edge à Intune**</span><span class="sxs-lookup"><span data-stu-id="a281e-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="a281e-112">[Configurer l’application dans Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="a281e-113">[Configurer les informations de l’application](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="a281e-114">[Configurer les paramètres de l’application](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="a281e-115">[Sélectionnez les balises d’étendue (facultatif)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="a281e-116">[Ajouter l’application](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="a281e-117">Pour plus d’informations, consultez [Résolution des problèmes](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="a281e-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




