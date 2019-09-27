---
title: Emplacement des données
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207259"
---
# <a name="data-location"></a><span data-ttu-id="c8e24-102">Emplacement des données</span><span class="sxs-lookup"><span data-stu-id="c8e24-102">Data location</span></span>

<span data-ttu-id="c8e24-103">Vous pouvez afficher l’emplacement de votre client Office 365 dans le centre d’administration ou en vous connectant à Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c8e24-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="c8e24-104">**Centre d’administration :**</span><span class="sxs-lookup"><span data-stu-id="c8e24-104">**Admin center:**</span></span>
1. <span data-ttu-id="c8e24-105">Connectez-vous au [Centre d’administration](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="c8e24-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="c8e24-106">Sélectionnez \*\*\*\* > **profil d’organisation**des paramètres.</span><span class="sxs-lookup"><span data-stu-id="c8e24-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="c8e24-107">Sous **emplacement des données**, sélectionnez **afficher les détails**.</span><span class="sxs-lookup"><span data-stu-id="c8e24-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="c8e24-108">**PowerShell**</span><span class="sxs-lookup"><span data-stu-id="c8e24-108">**PowerShell:**</span></span>
1. <span data-ttu-id="c8e24-109">Connectez-vous à Exchange Online à l’aide de Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c8e24-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="c8e24-110">Exécutez la cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) pour afficher la liste des propriétés de votre client.</span><span class="sxs-lookup"><span data-stu-id="c8e24-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="c8e24-111">Examinez la propriété PageY.</span><span class="sxs-lookup"><span data-stu-id="c8e24-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="c8e24-112">Lorsque vous disposez de l’emplacement des données pour EXO et SPO, vous pouvez déterminer l’emplacement des données pour les autres services que vous pouvez utiliser à l' [endroit où se trouvent vos données](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="c8e24-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>