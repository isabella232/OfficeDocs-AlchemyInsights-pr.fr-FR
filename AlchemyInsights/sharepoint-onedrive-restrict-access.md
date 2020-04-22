---
title: Restreindre l’accès dans SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692763"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="995fd-102">Restreindre l’accès dans SharePoint ou OneDrive</span><span class="sxs-lookup"><span data-stu-id="995fd-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="995fd-103">Il existe plusieurs façons de restreindre l’accès aux services SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="995fd-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="995fd-104">Ces différentes méthodes de restriction d’accès sont décrites ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="995fd-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="995fd-105">**Restriction des autorisations**</span><span class="sxs-lookup"><span data-stu-id="995fd-105">**Permission Restriction**</span></span>

<span data-ttu-id="995fd-106">Dans SharePoint Online et OneDrive entreprise, nous restreignons l’accès à des éléments tels que des sites, des fichiers et des dossiers en accordant uniquement l’accès à ces groupes/individus qui doivent avoir accès.</span><span class="sxs-lookup"><span data-stu-id="995fd-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="995fd-107">Personnaliser les autorisations pour une liste ou une bibliothèque SharePoint</span><span class="sxs-lookup"><span data-stu-id="995fd-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="995fd-108">Personnaliser les autorisations de site SharePoint</span><span class="sxs-lookup"><span data-stu-id="995fd-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="995fd-109">Modifier les autorisations sur un sous-dossier</span><span class="sxs-lookup"><span data-stu-id="995fd-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="995fd-110">Contrôler l’accès depuis des appareils enregistrés</span><span class="sxs-lookup"><span data-stu-id="995fd-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="995fd-111">En tant qu’administrateur SharePoint ou global, vous pouvez bloquer ou limiter l’accès au contenu SharePoint et OneDrive à partir d’appareils non gérés (ceux qui ne sont pas des services AD hybrides ou conformes dans Intune).</span><span class="sxs-lookup"><span data-stu-id="995fd-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="995fd-112">**Restriction d’emplacement réseau**</span><span class="sxs-lookup"><span data-stu-id="995fd-112">**Network Location Restriction**</span></span>

<span data-ttu-id="995fd-113">En tant qu’administrateur informatique, vous pouvez contrôler l’accès aux ressources SharePoint et OneDrive en fonction des emplacements réseau définis auxquels vous faites confiance.</span><span class="sxs-lookup"><span data-stu-id="995fd-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="995fd-114">C’est ce qu’on appelle aussi une stratégie basée sur l’emplacement.</span><span class="sxs-lookup"><span data-stu-id="995fd-114">This is also known as location-based policy.</span></span> <span data-ttu-id="995fd-115">Pour plus d’informations, reportez-vous à la rubrique [contrôler l’accès à SharePoint Online et aux données OneDrive en fonction de l’emplacement réseau](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="995fd-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="995fd-116">**Restriction de verrouillage de site**</span><span class="sxs-lookup"><span data-stu-id="995fd-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="995fd-117">Dans SharePoint Online, vous avez la possibilité de verrouiller une collection de sites, de sorte que personne ne puisse y accéder.</span><span class="sxs-lookup"><span data-stu-id="995fd-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="995fd-118">Cette valeur est définie via PowerShell et [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) à l’aide de la propriété [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="995fd-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="995fd-119">**Empêcher les utilisateurs de créer des sites ou des sous-sites**</span><span class="sxs-lookup"><span data-stu-id="995fd-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="995fd-120">En tant qu’administrateur SharePoint ou administrateur général, vous pouvez permettre à vos utilisateurs de créer et d’administrer leurs propres sites SharePoint, de déterminer le type de sites qu’ils peuvent créer et de spécifier l’emplacement des sites.</span><span class="sxs-lookup"><span data-stu-id="995fd-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="995fd-121">Pour plus d’informations, consultez la rubrique [gérer la création de sites dans SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation) .</span><span class="sxs-lookup"><span data-stu-id="995fd-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

