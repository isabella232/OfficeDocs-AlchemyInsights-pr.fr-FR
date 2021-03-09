---
title: Résoudre les problèmes d’installation MDATP sur un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568626"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="07a47-102">Résoudre les problèmes d’installation MDATP sur un Mac</span><span class="sxs-lookup"><span data-stu-id="07a47-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="07a47-103">En cas d’échec de l’installation manuelle, la page **Résumé** de l’Assistant Installation affiche l’erreur suivante :</span><span class="sxs-lookup"><span data-stu-id="07a47-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="07a47-104">« Une erreur s’est produite lors de l’installation.</span><span class="sxs-lookup"><span data-stu-id="07a47-104">"An error occurred during installation.</span></span> <span data-ttu-id="07a47-105">Le programme d’installation a rencontré une erreur qui a provoqué l’échec de l’installation.</span><span class="sxs-lookup"><span data-stu-id="07a47-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="07a47-106">Contactez le fabricant du logiciel pour obtenir de l’aide. »</span><span class="sxs-lookup"><span data-stu-id="07a47-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="07a47-107">Pour les déploiements mdm, la page affiche également un échec d’installation générique.</span><span class="sxs-lookup"><span data-stu-id="07a47-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="07a47-108">Bien que nous n’affichions pas d’erreurs exactes pour les utilisateurs finaux, nous tenez un fichier journal avec la progression de l’installation, dans **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="07a47-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="07a47-109">Chaque session d’installation s’y connecte.</span><span class="sxs-lookup"><span data-stu-id="07a47-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="07a47-110">Pour n’en sortie que la dernière session d’installation, utilisez `sed` .</span><span class="sxs-lookup"><span data-stu-id="07a47-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="07a47-111">Pour en savoir plus, voir Résoudre les problèmes [d’installation de Microsoft Defender ATP pour Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="07a47-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
