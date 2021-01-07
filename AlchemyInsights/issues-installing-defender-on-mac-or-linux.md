---
title: Problèmes d’installation de Microsoft Defender sur Mac ou Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768384"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="2f634-102">Problèmes d’installation de Microsoft Defender sur Mac ou Linux</span><span class="sxs-lookup"><span data-stu-id="2f634-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="2f634-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="2f634-103">**Mac**</span></span>

- <span data-ttu-id="2f634-104">Assurez-vous que la configuration requise est respectée avant d’installer Microsoft Defender ATP pour Mac.</span><span class="sxs-lookup"><span data-stu-id="2f634-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="2f634-105">Pour plus d’informations, voir [Installation de Microsoft Defender ATP pour Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="2f634-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="2f634-106">Examinez les informations du fichier : « /Library/Logs/Microsoft/mdatp/install.log ».</span><span class="sxs-lookup"><span data-stu-id="2f634-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="2f634-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="2f634-107">**Linux**</span></span>

- <span data-ttu-id="2f634-108">Assurez-vous que la configuration requise est respectée avant d’installer Microsoft Defender ATP pour Linux.</span><span class="sxs-lookup"><span data-stu-id="2f634-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="2f634-109">Pour plus d’informations, voir [Installation de Microsoft Defender ATP pour Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="2f634-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="2f634-110">Pour vérifier que le service MDATP est en cours d’exécution, voir [Échec de l’installation](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="2f634-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="2f634-111">Pour résoudre les problèmes si le service n’est pas en cours d’exécution, consultez [Étapes de résolution des problèmes si le service mdatp n’est pas en cours d’exécution](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="2f634-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="2f634-112">Pour connaître la procédure de vérification de la configuration du client, qui vérifie l’intégrité du produit, et d’exécution d’un test de détection sur le fichier texte EICAR, voir [Configuration du client](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="2f634-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="2f634-113">**Remarque** Pour obtenir la liste des systèmes de fichiers pris en charge pour l’activité à l’accès, voir [Microsoft Defender ATP pour Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="2f634-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>