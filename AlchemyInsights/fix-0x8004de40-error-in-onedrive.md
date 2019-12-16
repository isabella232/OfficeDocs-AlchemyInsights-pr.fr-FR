---
title: Corriger l’erreur 0x8004de40 dans OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052035"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="09f03-102">Corriger l’erreur 0x8004de40 dans OneDrive</span><span class="sxs-lookup"><span data-stu-id="09f03-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="09f03-103">Si vous recevez une erreur 0x8004de40 avec OneDrive :</span><span class="sxs-lookup"><span data-stu-id="09f03-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="09f03-104">Redémarrez l’ordinateur concerné en étant connecté à votre domaine d’annuaire acitve.</span><span class="sxs-lookup"><span data-stu-id="09f03-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="09f03-105">Si un redémarrage ne résout pas le problème, Déjoignez et rejoignez votre appareil à partir d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09f03-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="09f03-106">**Remarque**: vous devez être sur votre réseau d’entreprise tout en effectuant ces étapes.</span><span class="sxs-lookup"><span data-stu-id="09f03-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="09f03-107">N’effectuez pas ces étapes Lorsque vous ne parvenez pas à vous connecter à votre infrastructure d’entreprise (par exemple, lors de vos déplacements).</span><span class="sxs-lookup"><span data-stu-id="09f03-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="09f03-108">Ouvrez une invite de commandes avec élévation de privilèges.</span><span class="sxs-lookup"><span data-stu-id="09f03-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="09f03-109">Pour ouvrir une invite de commandes avec élévation de privilèges, cliquez sur- **Démarrer**, cliquez avec le bouton droit sur **invite de commandes**, puis cliquez sur **exécuter en tant qu’administrateur**.</span><span class="sxs-lookup"><span data-stu-id="09f03-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="09f03-110">Tapez *dsregcmd/Leave* , puis appuyez sur **entrée**.</span><span class="sxs-lookup"><span data-stu-id="09f03-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="09f03-111">Lorsque vous avez terminé, tapez *dsregcmd/Join* , puis appuyez sur **entrée**.</span><span class="sxs-lookup"><span data-stu-id="09f03-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="09f03-112">Lorsque vous avez terminé, fermez l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="09f03-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="09f03-113">Redémarrez l’ordinateur, puis connectez-vous à OneDrive.</span><span class="sxs-lookup"><span data-stu-id="09f03-113">Reboot the computer, and log into OneDrive.</span></span>