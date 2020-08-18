---
title: Modifier les canaux de mise à jour pour les applications Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 43a3cdefe5a9bc1726984a3195dce7aaea08d892
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786851"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="87725-102">Modifier les canaux de mise à jour pour les applications Office</span><span class="sxs-lookup"><span data-stu-id="87725-102">Change update channels for Office apps</span></span>

<span data-ttu-id="87725-103">Pour les nouvelles installations Office, utilisez les paramètres de téléchargement du logiciel Office pour sélectionner le canal de mise à jour souhaité, puis installez (ou réinstallez) les applications Office.</span><span class="sxs-lookup"><span data-stu-id="87725-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="87725-104">Pour plus d’informations, consultez [Gérer les paramètres de téléchargement des logiciels dans Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="87725-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="87725-105">**Remarque** le canal de mise à jour sélectionné à l’aide des paramètres de téléchargement du logiciel Office s’applique à tous les utilisateurs effectuant de nouvelles installations à l’aide du Portail Office 365.</span><span class="sxs-lookup"><span data-stu-id="87725-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="87725-106">Pour plus d’informations, consultez [Télécharger et installer ou réinstaller Microsoft 365 ou Office 2019 sur un PC ou Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="87725-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="87725-107">Pour les installations Office existantes, utilisez l’outil Déploiement d’Office (ODT) pour basculer vers un autre canal de mise à jour :</span><span class="sxs-lookup"><span data-stu-id="87725-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="87725-108">Téléchargez la dernière version de l’outil de Déploiement d’Office (setup.exe) à partir du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="87725-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="87725-109">Identifiez le nom du canal vers lequel vous voulez basculer.</span><span class="sxs-lookup"><span data-stu-id="87725-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="87725-110">Pour plus d’informations, consultez [Options de configuration pour l’outil déploiement d’Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="87725-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="87725-111">Créez un fichier XML de configuration spécifiant le nom du canal approprié (par exemple, update.xml).</span><span class="sxs-lookup"><span data-stu-id="87725-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="87725-112">À partir d’une invite de commandes avec élévation de privilèges, basculez vers l’emplacement du dossier où setup.exe réside et exécutez la commande suivante :</span><span class="sxs-lookup"><span data-stu-id="87725-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="87725-113">a.</span><span class="sxs-lookup"><span data-stu-id="87725-113">a.</span></span> <span data-ttu-id="87725-114">setup.exe /configurer update.xml</span><span class="sxs-lookup"><span data-stu-id="87725-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="87725-115">Lancez une application Office (par exemple, Excel), puis sélectionnez **Fichier** > **Compte**.</span><span class="sxs-lookup"><span data-stu-id="87725-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="87725-116">Dans la section Informations sur le produit, sélectionnez **Options de mise à jour** > **Mettre à jour**.</span><span class="sxs-lookup"><span data-stu-id="87725-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="87725-117">Pour plus d’informations, consultez [Comment changer les canaux de mise à jour des applications Office existantes](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="87725-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="87725-118">Pour changer les canaux de mise à jour pour un groupe d’utilisateurs sélectionné ou à l’aide de Gestionnaire de configuration (SCCM), configurez le paramètre de canal de mise à jour à l’aide de GPO.</span><span class="sxs-lookup"><span data-stu-id="87725-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="87725-119">Si vous souhaitez pour plus d’informations, consultez la rubrique relative à la [Présentation des canaux de mise à jour pour Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="87725-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="87725-120">Pour plus d’informations, consultez les rubriques [Comment gérer les canaux Office 365 ProPlus pour les professionnels de l’informatique](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) et [Gérer les mises à jour vers Microsoft 365 Apps avec Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="87725-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>