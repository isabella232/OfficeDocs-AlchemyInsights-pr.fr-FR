---
title: Supprimer le service d’arrière-plan pour la Recherche Microsoft dans Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753414"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="fadf1-102">Supprimer le service d’arrière-plan pour la Recherche Microsoft dans Bing</span><span class="sxs-lookup"><span data-stu-id="fadf1-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="fadf1-103">Pour supprimer le service d’arrière-plan pour Recherche Microsoft dans Bing, vous pouvez essayer ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="fadf1-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="fadf1-104">Pour revenir aux paramètres du moteur de recherche d’origine, vous pouvez effectuer les opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="fadf1-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="fadf1-105">a.</span><span class="sxs-lookup"><span data-stu-id="fadf1-105">a.</span></span> <span data-ttu-id="fadf1-106">Commutez le **[bouton bascule](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Utiliser Bing comme moteur de recherche par défaut sur Désactivé**.</span><span class="sxs-lookup"><span data-stu-id="fadf1-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="fadf1-107">b.</span><span class="sxs-lookup"><span data-stu-id="fadf1-107">b.</span></span> <span data-ttu-id="fadf1-108">[Accédez au Centre d’administration Microsoft 365,](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) et effacez le paramètre qui affecte tous les utilisateurs de votre organisation.</span><span class="sxs-lookup"><span data-stu-id="fadf1-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="fadf1-109">Pour supprimer le service d’arrière-plan d’un appareil individuel, effectuer les tâches suivantes :</span><span class="sxs-lookup"><span data-stu-id="fadf1-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="fadf1-110">a.</span><span class="sxs-lookup"><span data-stu-id="fadf1-110">a.</span></span> <span data-ttu-id="fadf1-111">Sélectionnez **Panneau de configuration > Programmes > Programmes et fonctionnalités**.</span><span class="sxs-lookup"><span data-stu-id="fadf1-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="fadf1-112">b.</span><span class="sxs-lookup"><span data-stu-id="fadf1-112">b.</span></span> <span data-ttu-id="fadf1-113">Cliquez avec le bouton **Recherche Microsoft dans Bing** sous la liste des programmes installés, puis cliquez sur **Désinstaller**.</span><span class="sxs-lookup"><span data-stu-id="fadf1-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="fadf1-114">Pour supprimer le service d’arrière-plan de plusieurs appareils dans votre organisation, connectez-vous en tant qu’administrateur et exécutez la commande suivante dans un script :</span><span class="sxs-lookup"><span data-stu-id="fadf1-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
