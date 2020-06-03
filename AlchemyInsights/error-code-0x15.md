---
title: Code d’erreur 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506844"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="0b60a-103">Erreur lors de l’activation d’Office 2013 sur les services Bureau à distance</span><span class="sxs-lookup"><span data-stu-id="0b60a-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="0b60a-104">Si vous recevez une erreur lors de l’activation d’Office 2013 sur les déploiements des services Bureau à distance (RDS), envisagez d’activer ADAL en modifiant le registre.</span><span class="sxs-lookup"><span data-stu-id="0b60a-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="0b60a-105">**Clé de Registre**</span><span class="sxs-lookup"><span data-stu-id="0b60a-105">**Registry key**</span></span>|<span data-ttu-id="0b60a-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="0b60a-106">**Type**</span></span>|<span data-ttu-id="0b60a-107">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0b60a-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0b60a-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="0b60a-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="0b60a-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="0b60a-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="0b60a-110">1 </span><span class="sxs-lookup"><span data-stu-id="0b60a-110">1</span></span>  <br/> |

<span data-ttu-id="0b60a-111">Pour plus d’informations, consultez la rubrique [activer l’authentification moderne pour Office 2013 sur les appareils Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="0b60a-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="0b60a-112">ADAL est activée par défaut dans les applications Microsoft 365 pour entreprise et Office 2016.</span><span class="sxs-lookup"><span data-stu-id="0b60a-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="0b60a-113">Services Bureau à distance (RDS) était précédemment nommé services Terminal Server.</span><span class="sxs-lookup"><span data-stu-id="0b60a-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  