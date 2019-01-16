---
title: L’installation d’office sur un serveur Terminal Server - sans licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288426"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="6143a-102">Installez Office sur un serveur Terminal Server</span><span class="sxs-lookup"><span data-stu-id="6143a-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="6143a-103">Pour le déploiement d’Office 365 ProPlus sur un serveur Windows à l’aide de Remote Desktop Services (RDS), anciennement Services Terminal Server :</span><span class="sxs-lookup"><span data-stu-id="6143a-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="6143a-p101">Vous devez disposer d’un plan Office 365 qui inclut Office 365 ProPlus, telles que Office 365 entreprise E3 ou entreprise E5. Les plans Office 365 entreprise et Office 365 entreprise Premium n’incluent pas Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="6143a-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="6143a-106">Vous devez activer [l’activation de l’ordinateur partagé](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6143a-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="6143a-107">Si vous souhaitez installer Office 365 ProPlus à partir du portail Office 365, sur RDS \*\* *qui utilise les paramètres d’installation par défaut* \*\*, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="6143a-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="6143a-p102">Vérifier quels plan Office 365 que vous avez. [Découvrez comment](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="6143a-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="6143a-p103">Si nécessaire, basculez vers un autre Office 365 planifier. [Découvrez comment](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="6143a-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="6143a-p104">Si Office est déjà installé sur le serveur RDS à l’aide de tous les autres plans Office 365, désinstallez-la. Par exemple, en accédant au panneau \> désinstaller un programme. Désinstallation à l’aide de [l’Assistant de récupération et de prise en charge de Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous utilisez des problèmes.</span><span class="sxs-lookup"><span data-stu-id="6143a-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="6143a-115">Sur le serveur RDS, connectez-vous au portail Office 365 avec votre compte d’administrateur et [installez Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="6143a-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="6143a-116">Une fois Office est installé, \*\* *ne pas ouvrir ou connectez-vous* \*\* pour toutes les applications Office.</span><span class="sxs-lookup"><span data-stu-id="6143a-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="6143a-117">Sur le serveur RDS, activer un ordinateur partagé en modifiant le Registre en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="6143a-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="6143a-p105">Cliquez sur le bouton Windows dans l’angle inférieur gauche de votre écran, puis sélectionnez Exécuter. Dans la zone Ouvrir, tapez **regedit**, puis sélectionnez OK.</span><span class="sxs-lookup"><span data-stu-id="6143a-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="6143a-120">Sélectionnez Oui lorsque vous êtes invité à autoriser l’Éditeur du Registre pour apporter des modifications à votre appareil.</span><span class="sxs-lookup"><span data-stu-id="6143a-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="6143a-121">Dans l’Éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec la valeur 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="6143a-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="6143a-122">Sur le serveur RDS, \*\* *se connecter en tant qu’un utilisateur final* \*\* et [Vérifiez que l’activation de l’ordinateur partagé est activé pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="6143a-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="6143a-123">Pour plus d’informations sur les conditions préalables, des instructions d’installation et des conseils sur les installations personnalisées à l’aide de l’outil de déploiement d’Office, consultez [Déploiement d’Office 365 ProPlus à l’aide des Services Bureau à distance](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="6143a-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="6143a-124">Pour corriger les erreurs liées à l’activation de l’ordinateur partagé, consultez [résoudre les problèmes liés à l’activation d’un ordinateur partagé pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="6143a-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

