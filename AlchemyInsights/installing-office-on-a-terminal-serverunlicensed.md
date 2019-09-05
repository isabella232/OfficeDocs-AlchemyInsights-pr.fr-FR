---
title: Installation d’Office sur un serveur Terminal Server sans licence
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735387"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="4a397-102">Installation d’Office sur un serveur Terminal Server</span><span class="sxs-lookup"><span data-stu-id="4a397-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="4a397-103">Pour déployer Office 365 ProPlus sur un serveur Windows à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :</span><span class="sxs-lookup"><span data-stu-id="4a397-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="4a397-104">Vous devez disposer d’un plan Office 365 qui inclut Office 365 ProPlus, comme Office 365 entreprise E3 ou entreprise E5.</span><span class="sxs-lookup"><span data-stu-id="4a397-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="4a397-105">Les plans Office 365 Business et Office 365 Business Premium n’incluent pas Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="4a397-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="4a397-106">Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4a397-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="4a397-107">Si vous souhaitez installer Office 365 ProPlus sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="4a397-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="4a397-108">Consultez la planification d’Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a397-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="4a397-109">Découvrez comment</span><span class="sxs-lookup"><span data-stu-id="4a397-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="4a397-110">Si nécessaire, passez à une autre offre Office 365.</span><span class="sxs-lookup"><span data-stu-id="4a397-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="4a397-111">Découvrez comment</span><span class="sxs-lookup"><span data-stu-id="4a397-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="4a397-112">Si Office est déjà installé sur le serveur RDS à l’aide d’autres plans Office 365, désinstallez-le.</span><span class="sxs-lookup"><span data-stu-id="4a397-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="4a397-113">Par exemple, en accédant à panneau \> de configuration désinstaller un programme.</span><span class="sxs-lookup"><span data-stu-id="4a397-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="4a397-114">Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.</span><span class="sxs-lookup"><span data-stu-id="4a397-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="4a397-115">Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [installez Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="4a397-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="4a397-116">Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.</span><span class="sxs-lookup"><span data-stu-id="4a397-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="4a397-117">Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="4a397-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="4a397-118">Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez Exécuter.</span><span class="sxs-lookup"><span data-stu-id="4a397-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="4a397-119">Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur OK.</span><span class="sxs-lookup"><span data-stu-id="4a397-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="4a397-120">Sélectionnez Oui lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.</span><span class="sxs-lookup"><span data-stu-id="4a397-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="4a397-121">Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="4a397-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="4a397-122">Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="4a397-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="4a397-123">Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy office 365 ProPlus à l’aide des services Bureau à distance](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="4a397-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="4a397-124">Pour résoudre les erreurs liées à l’activation d’ordinateurs partagés, voir [résoudre les problèmes liés à l’activation d’ordinateurs partagés pour Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="4a397-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  