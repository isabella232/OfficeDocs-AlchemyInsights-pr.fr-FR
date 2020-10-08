---
title: Déploiement d’applications Win32 avec Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366506"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="35ea7-102">Déploiement d’applications Win32 avec Intune</span><span class="sxs-lookup"><span data-stu-id="35ea7-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="35ea7-103">Microsoft Intune autorise les applications Win32, y compris, mais non limitées aux applications MSI et .EXE à déployer sur les appareils Windows 10.</span><span class="sxs-lookup"><span data-stu-id="35ea7-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="35ea7-104">Le mécanisme de déploiement utilisé nécessite que l’IME (Intune Management Extension) soit présente sur l’appareil cible.</span><span class="sxs-lookup"><span data-stu-id="35ea7-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="35ea7-105">L’IME est installée automatiquement suite au ciblage d’un script PowerShell ou d’une application Win32 sur un utilisateur/appareil.</span><span class="sxs-lookup"><span data-stu-id="35ea7-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="35ea7-106">Il existe également une série de conditions préalables devant être remplies pour déployer les applications Win32, notamment :</span><span class="sxs-lookup"><span data-stu-id="35ea7-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="35ea7-107">Plateformes prises en charge : Windows 10 version 1607 ou ultérieure (versions Entreprise, Pro et Éducation).</span><span class="sxs-lookup"><span data-stu-id="35ea7-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="35ea7-108">Architecture non prise en charge : x86 et x64.</span><span class="sxs-lookup"><span data-stu-id="35ea7-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="35ea7-109">Gestion des appareils : AAD joint et inscrit automatiquement (y compris les jointures de domaines hybrides et les stratégies de groupe inscrites automatiquement).</span><span class="sxs-lookup"><span data-stu-id="35ea7-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="35ea7-110">Format du package d’application : fichier .**intunewin** préparé par l’[outil de préparation de contenu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="35ea7-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="35ea7-111">Limites :</span><span class="sxs-lookup"><span data-stu-id="35ea7-111">Limitations:</span></span>
    - <span data-ttu-id="35ea7-112">Taille maximale : 8 Go.</span><span class="sxs-lookup"><span data-stu-id="35ea7-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="35ea7-113">Architecture non prise en charge : ARM.</span><span class="sxs-lookup"><span data-stu-id="35ea7-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="35ea7-114">Consultez le document [Ajouter, attribuer et surveiller une application Win32 dans Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add) pour plus d’informations sur ces étapes.</span><span class="sxs-lookup"><span data-stu-id="35ea7-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="35ea7-115">Pour plus d’informations sur la résolution des problèmes de déploiement des applications sur Windows, notamment les applications Win32, suivez les documents suivants :</span><span class="sxs-lookup"><span data-stu-id="35ea7-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="35ea7-116">Résoudre les problèmes d’installation d’application</span><span class="sxs-lookup"><span data-stu-id="35ea7-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="35ea7-117">Résoudre les problèmes liés aux applications Win32</span><span class="sxs-lookup"><span data-stu-id="35ea7-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)