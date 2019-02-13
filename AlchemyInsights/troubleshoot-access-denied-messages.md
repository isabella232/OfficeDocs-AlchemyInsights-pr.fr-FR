---
title: Résolution des messages d’accès refusé
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: f1a4803838b6511ef4fe7f03cafa4aa13b3c9734
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916450"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="f08e0-102">Résolution des messages d’accès refusé</span><span class="sxs-lookup"><span data-stu-id="f08e0-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="f08e0-p101">Si une personne a obtenu un message « Accès refusé » dans un dossier partagé, l’administrateur de collection de sites avez activé « accès limité utilisateur autorisation mode verrouillage. » Pour désactiver cette option :</span><span class="sxs-lookup"><span data-stu-id="f08e0-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="f08e0-105">Accédez au site, cliquez sur l’icône Paramètres, puis cliquez sur **Paramètres du Site**.</span><span class="sxs-lookup"><span data-stu-id="f08e0-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="f08e0-106">Sous **Administration de la collection de sites**, cliquez sur **Fonctionnalités de la collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="f08e0-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="f08e0-107">En regard de **mode de verrouillage autorisation accès limité utilisateur**, cliquez sur **désactiver**.</span><span class="sxs-lookup"><span data-stu-id="f08e0-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="f08e0-p102">Un message accès refusé peut également se produire pour les dossiers partagés si le site est un site de publication. Pour obtenir des informations, consultez [Accès refusé lorsque vous accédez à un dossier partagé](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="f08e0-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="f08e0-p103">Si une personne a obtenu un message « Accès refusé » lorsque vous essayez d’afficher les demandes d’accès, l’utilisateur doit être ajouté en tant que membre du groupe propriétaires du site soit un administrateur de collection de sites. Pour plus d’informations, consultez [Accès refusé à la liste des demandes d’accès](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="f08e0-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="f08e0-112">Si un utilisateur a obtenu un message « Accès refusé » après que qu’ils ont été supprimés d’Active Directory sur site et puis rajoutés, consultez [Accès refusé lorsqu’un compte d’utilisateur est synchronisé avec Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="f08e0-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

