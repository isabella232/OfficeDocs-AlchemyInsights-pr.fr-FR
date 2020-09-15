---
title: Installation d’Office sur un serveur Terminal Server sans licence
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663115"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="552f1-102">Installation d’Office sur un serveur Terminal Server</span><span class="sxs-lookup"><span data-stu-id="552f1-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="552f1-103">Pour déployer des applications Microsoft 365 pour Enterprise sur un serveur Windows à l’aide des services Bureau à distance (RDS), anciennement services Terminal Server :</span><span class="sxs-lookup"><span data-stu-id="552f1-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="552f1-104">Vous devez disposer d’un abonnement Microsoft 365 qui inclut les applications Microsoft 365 pour les entreprises, comme Office 365 entreprise E3 ou entreprise E5.</span><span class="sxs-lookup"><span data-stu-id="552f1-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="552f1-105">Les applications Microsoft 365 Apps for Business et Microsoft 365 pour les offres Business Premium n’incluent pas les applications Microsoft 365 pour les entreprises.</span><span class="sxs-lookup"><span data-stu-id="552f1-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="552f1-106">Vous devez activer [l’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="552f1-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="552f1-107">Si vous souhaitez installer Microsoft 365 apps pour Enterprise sur RDS à partir du centre d’administration de Microsoft 365, ***qui utilise les paramètres d’installation par défaut***, procédez comme suit.</span><span class="sxs-lookup"><span data-stu-id="552f1-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="552f1-108">Vous pouvez également télécharger et exécuter l' [Assistant support et récupération Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) pour installer les applications Microsoft 365 pour Enterprise en mode d’activation d’ordinateur partagé.</span><span class="sxs-lookup"><span data-stu-id="552f1-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="552f1-109">Vérifiez l’abonnement Microsoft 365 que vous avez.</span><span class="sxs-lookup"><span data-stu-id="552f1-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="552f1-110">Découvrez comment</span><span class="sxs-lookup"><span data-stu-id="552f1-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="552f1-111">Si nécessaire, passez à un autre abonnement Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="552f1-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="552f1-112">Découvrez comment</span><span class="sxs-lookup"><span data-stu-id="552f1-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="552f1-113">Si Office est déjà installé sur le serveur RDS à l’aide d’autres abonnements Microsoft 365, désinstallez-le.</span><span class="sxs-lookup"><span data-stu-id="552f1-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="552f1-114">Par exemple, en accédant à panneau de configuration \> désinstaller un programme.</span><span class="sxs-lookup"><span data-stu-id="552f1-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="552f1-115">Désinstallation à l’aide [de l’Assistant support et récupération Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) si vous rencontrez des problèmes.</span><span class="sxs-lookup"><span data-stu-id="552f1-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="552f1-116">Sur le serveur RDS, connectez-vous au centre d’administration Microsoft 365 avec votre compte d’administrateur et [Installez microsoft 365 apps pour entreprises](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="552f1-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="552f1-117">Une fois Office installé, ***ne pas ouvrir ou se connecter*** à une application Office.</span><span class="sxs-lookup"><span data-stu-id="552f1-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="552f1-118">Sur le serveur RDS, activez l’activation d’ordinateurs partagés en modifiant le registre en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="552f1-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="552f1-119">Cliquez avec le bouton droit sur le bouton Windows dans le coin inférieur gauche de votre écran et sélectionnez Exécuter.</span><span class="sxs-lookup"><span data-stu-id="552f1-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="552f1-120">Dans la zone Ouvrir, tapez **regedit**, puis cliquez sur OK.</span><span class="sxs-lookup"><span data-stu-id="552f1-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="552f1-121">Sélectionnez Oui lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.</span><span class="sxs-lookup"><span data-stu-id="552f1-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="552f1-122">Dans l’éditeur du Registre, ajoutez une valeur de chaîne de **SharedComputerLicensing** avec un paramètre de 1 sous HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="552f1-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="552f1-123">Sur le serveur RDS, ***Connectez-vous en tant qu’utilisateur final*** et [Vérifiez que l’activation d’ordinateurs partagés est activée pour les applications Microsoft 365 pour entreprises](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="552f1-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="552f1-124">Pour plus d’informations sur les conditions préalables, les instructions de configuration et des conseils sur les installations personnalisées à l’aide de l’outil déploiement d’Office, consultez la rubrique [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="552f1-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="552f1-125">Pour résoudre les erreurs liées à l’activation d’ordinateurs partagés, consultez la rubrique [Troubleshoot Problems with Shared Computer activation for Microsoft 365 Apps for Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="552f1-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  