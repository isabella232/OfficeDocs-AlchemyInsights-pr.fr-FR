---
title: Code d’erreur 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements Remote Desktop Services (RDS), envisagez d’activer ADAL en modifiant le Registre.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499380"
---
<span data-ttu-id="12c4b-103">Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements Remote Desktop Services (RDS), envisagez d’activer ADAL en modifiant le Registre.</span><span class="sxs-lookup"><span data-stu-id="12c4b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="12c4b-104">**Clé de Registre**</span><span class="sxs-lookup"><span data-stu-id="12c4b-104">**Registry key**</span></span>|<span data-ttu-id="12c4b-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="12c4b-105">**Type**</span></span>|<span data-ttu-id="12c4b-106">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="12c4b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="12c4b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="12c4b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="12c4b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="12c4b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="12c4b-109">^1</span><span class="sxs-lookup"><span data-stu-id="12c4b-109">1</span></span>  <br/> |
   
<span data-ttu-id="12c4b-110">Pour plus d’informations, voir [Activer l’authentification moderne pour Office 2013 sur les périphériques Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="12c4b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="12c4b-p101">ADAL est activée par défaut dans Office 365 ProPlus et Office 2016. > remote Desktop Services (RDS) a été précédemment appelé Services Terminal Server.</span><span class="sxs-lookup"><span data-stu-id="12c4b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

