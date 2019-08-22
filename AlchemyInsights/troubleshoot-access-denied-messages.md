---
title: Résoudre les problèmes de refus d’accès aux messages
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500401"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f2eb6-102">Résoudre les problèmes de refus d’accès aux messages</span><span class="sxs-lookup"><span data-stu-id="f2eb6-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f2eb6-103">Si un utilisateur a reçu un message «accès refusé» à un dossier partagé dans SharePoint, il est possible que l’administrateur de collection de sites ait activé le mode de verrouillage des autorisations utilisateur à accès limité.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="f2eb6-104">Pour désactiver cette fonctionnalité, procédez comme suit:</span><span class="sxs-lookup"><span data-stu-id="f2eb6-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="f2eb6-105">Accédez au site, cliquez sur l’icône Paramètres, puis cliquez sur **paramètres du site**.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f2eb6-106">Sous **Administration de la collection de sites**, cliquez sur **Fonctionnalités de la collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f2eb6-107">En regard de **mode de verrouillage des autorisations utilisateur avec accès limité**, cliquez sur **Désactiver**.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f2eb6-108">Un message de refus d’accès peut également se produire pour les dossiers partagés s’il s’agit d’un site de publication.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="f2eb6-109">Pour plus d’informations, consultez [la rubrique accès refusé lors de l’accès à un dossier partagé](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="f2eb6-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="f2eb6-110">Si une personne a reçu un message de type «accès refusé» lors de la tentative d’affichage des demandes d’accès, il doit être ajouté en tant qu’administrateur de collection de sites ou en tant que membre du groupe propriétaires pour le site.</span><span class="sxs-lookup"><span data-stu-id="f2eb6-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="f2eb6-111">Pour plus d’informations, consultez la rubrique [accès refusé à la liste des demandes d’accès](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f2eb6-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f2eb6-112">Si un utilisateur a reçu un message «accès refusé» une fois qu’il a été supprimé d’Active Directory en local, puis rajouté, consultez [la rubrique accès refusé lorsqu’un compte d’utilisateur est synchronisé avec Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f2eb6-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

