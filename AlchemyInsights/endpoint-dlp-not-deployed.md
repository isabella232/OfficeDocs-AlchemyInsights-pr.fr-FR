---
title: DLP de point de terminaison non déployé sur l’appareil de l’utilisateur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52694805"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="702bd-102">DLP de point de terminaison non déployé sur l’appareil de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="702bd-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="702bd-103">Si le paramètre de protection contre la perte de données (DLP) du point de terminaison ne s’est pas appliqué à l’appareil d’un utilisateur, vérifiez que vous répondez aux exigences suivantes :protection contre la perte de données :</span><span class="sxs-lookup"><span data-stu-id="702bd-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="702bd-104">Windows 10 x64 build 1809 ou une version ultérieure est installé sur l'appareil.</span><span class="sxs-lookup"><span data-stu-id="702bd-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="702bd-105">Le client anti-programme malveillant version 4.18.2009.7 ou version ultérieure est installé.</span><span class="sxs-lookup"><span data-stu-id="702bd-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="702bd-106">L’appareil est **l’un** des suivants :</span><span class="sxs-lookup"><span data-stu-id="702bd-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="702bd-107">Jointure Azure Active Directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="702bd-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="702bd-108">Jointure hybride Azure AD</span><span class="sxs-lookup"><span data-stu-id="702bd-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="702bd-109">Inscrit à AAD</span><span class="sxs-lookup"><span data-stu-id="702bd-109">AAD registered</span></span>

- <span data-ttu-id="702bd-110">Pour appliquer des actions de stratégie, assurez-vous que le navigateur Microsoft Chromium Edge est installé sur l’appareil du point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="702bd-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="702bd-111">Pour plus d’informations sur la configuration requise pour le déploiement de la protection contre la perte de données de point de terminaison, consultez [Prise en main la protection contre la perte de données de point de terminaison](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="702bd-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>