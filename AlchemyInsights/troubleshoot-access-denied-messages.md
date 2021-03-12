---
title: Résoudre les problèmes de messages d’accès refusé
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704892"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="70ab8-102">Résoudre les problèmes de messages d’accès refusé</span><span class="sxs-lookup"><span data-stu-id="70ab8-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="70ab8-103">Si quelqu’un a reçu un message « Accès refusé » dans un dossier partagé dans SharePoint, l’administrateur de la collection de sites a peut-être activé le « mode de verrouillage des autorisations utilisateur à accès limité ».</span><span class="sxs-lookup"><span data-stu-id="70ab8-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="70ab8-104">Pour désactiver cette situation :</span><span class="sxs-lookup"><span data-stu-id="70ab8-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="70ab8-105">Accédez au site, cliquez sur l’icône Paramètres, puis cliquez sur **Paramètres du site.**</span><span class="sxs-lookup"><span data-stu-id="70ab8-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="70ab8-106">Sous **Administration de la collection de sites**, cliquez sur **Fonctionnalités de la collection de sites**.</span><span class="sxs-lookup"><span data-stu-id="70ab8-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="70ab8-107">En plus du **mode verrouillage d’autorisation** utilisateur à accès limité, cliquez **sur Désactiver.**</span><span class="sxs-lookup"><span data-stu-id="70ab8-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="70ab8-108">Un message de refus d’accès peut également se produire pour les dossiers partagés si le site est un site de publication.</span><span class="sxs-lookup"><span data-stu-id="70ab8-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="70ab8-109">Pour plus d’informations, [voir Accès refusé lors de l’accès à un dossier partagé.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="70ab8-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="70ab8-110">Si une personne a reçu un message « Accès refusé » lors de la tentative d’affichage des demandes d’accès, l’utilisateur doit être ajouté en tant qu’administrateur de collection de sites ou membre du groupe Propriétaires du site.</span><span class="sxs-lookup"><span data-stu-id="70ab8-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="70ab8-111">Pour plus d’informations, [consultez la liste Demandes d’accès refusées.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="70ab8-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="70ab8-112">Si un utilisateur a reçu un message « Accès refusé » après qu’il a été supprimé d’Active Directory local, puis ajouté à nouveau, voir Accès refusé lorsqu’un compte d’utilisateur est synchronisé avec [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="70ab8-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

