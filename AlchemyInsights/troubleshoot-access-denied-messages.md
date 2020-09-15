---
title: Résoudre les problèmes de refus d’accès aux messages
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690781"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="e0406-102">Résoudre les problèmes de refus d’accès aux messages</span><span class="sxs-lookup"><span data-stu-id="e0406-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="e0406-103">Si un utilisateur a reçu un message « accès refusé » à un dossier partagé dans SharePoint, il est possible que l’administrateur de collection de sites ait activé le mode de verrouillage des autorisations utilisateur à accès limité.</span><span class="sxs-lookup"><span data-stu-id="e0406-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="e0406-104">Pour désactiver cette fonctionnalité, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="e0406-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="e0406-105">Accédez au site, cliquez sur l’icône Paramètres, puis cliquez sur **paramètres du site**.</span><span class="sxs-lookup"><span data-stu-id="e0406-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="e0406-106">Sous **Administration de la collection de sites**, cliquez sur **Fonctionnalités de la collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="e0406-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="e0406-107">En regard de **mode de verrouillage des autorisations utilisateur avec accès limité**, cliquez sur **Désactiver**.</span><span class="sxs-lookup"><span data-stu-id="e0406-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="e0406-108">Un message de refus d’accès peut également se produire pour les dossiers partagés s’il s’agit d’un site de publication.</span><span class="sxs-lookup"><span data-stu-id="e0406-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="e0406-109">Pour plus d’informations, consultez [la rubrique accès refusé lors de l’accès à un dossier partagé](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="e0406-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="e0406-110">Si une personne a reçu un message de type « accès refusé » lors de la tentative d’affichage des demandes d’accès, il doit être ajouté en tant qu’administrateur de collection de sites ou en tant que membre du groupe propriétaires pour le site.</span><span class="sxs-lookup"><span data-stu-id="e0406-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="e0406-111">Pour plus d’informations, consultez la rubrique [accès refusé à la liste des demandes d’accès](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="e0406-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="e0406-112">Si un utilisateur a reçu un message « accès refusé » une fois qu’il a été supprimé d’Active Directory en local, puis rajouté, consultez [la rubrique accès refusé lorsqu’un compte d’utilisateur est synchronisé avec Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="e0406-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

