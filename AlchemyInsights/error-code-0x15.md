---
title: Code d’erreur 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388243"
---
<span data-ttu-id="51b1e-103">Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.</span><span class="sxs-lookup"><span data-stu-id="51b1e-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="51b1e-104">**Clé de Registre**</span><span class="sxs-lookup"><span data-stu-id="51b1e-104">**Registry key**</span></span>|<span data-ttu-id="51b1e-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="51b1e-105">**Type**</span></span>|<span data-ttu-id="51b1e-106">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="51b1e-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="51b1e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="51b1e-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="51b1e-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="51b1e-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="51b1e-109">0,1</span><span class="sxs-lookup"><span data-stu-id="51b1e-109">1</span></span>  <br/> |

<span data-ttu-id="51b1e-110">Pour plus d’informations, consultez la rubrique [activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="51b1e-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="51b1e-111">ADAL est activée par défaut dans Office 365 ProPlus et Office 2016.</span><span class="sxs-lookup"><span data-stu-id="51b1e-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="51b1e-112">> services Bureau à distance (RDS) était précédemment nommé services Terminal Server.</span><span class="sxs-lookup"><span data-stu-id="51b1e-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  