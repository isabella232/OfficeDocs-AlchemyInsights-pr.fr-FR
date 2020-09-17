---
title: 932 mise à niveau de AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806037"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="f0724-102">Mettre à niveau Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="f0724-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="f0724-103">Par défaut, la mise à niveau automatique est activée pour Azure AD Connect, ce qui permet de s’assurer que vous utilisez la dernière version.</span><span class="sxs-lookup"><span data-stu-id="f0724-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="f0724-104">Pour vérifier les paramètres de mise à niveau automatique, utilisez la cmdlet **Get-ADSyncAutoUpgrade** dans Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f0724-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="f0724-105">L’applet de commande renvoie l’une des valeurs suivantes :</span><span class="sxs-lookup"><span data-stu-id="f0724-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="f0724-106">**Activé**: la mise à niveau automatique est activée.</span><span class="sxs-lookup"><span data-stu-id="f0724-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="f0724-107">**Désactivé**: la mise à niveau automatique est désactivée.</span><span class="sxs-lookup"><span data-stu-id="f0724-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="f0724-108">**Suspendu**: le système n’est plus autorisé à recevoir des mises à niveau automatiques.</span><span class="sxs-lookup"><span data-stu-id="f0724-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="f0724-109">Vous ne pouvez pas configurer cette valeur ; elle est définie par le système.</span><span class="sxs-lookup"><span data-stu-id="f0724-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="f0724-110">Pour plus d’informations, consultez la rubrique [mise à niveau automatique](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="f0724-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="f0724-111">Pour télécharger la dernière version d’Azure AD Connect, accédez à [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="f0724-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
