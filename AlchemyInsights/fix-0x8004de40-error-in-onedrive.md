---
title: Corriger 0x8004de40'erreur dans OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649746"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="14887-102">Corriger 0x8004de40'erreur dans OneDrive</span><span class="sxs-lookup"><span data-stu-id="14887-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="14887-103">Si vous exécutez Windows 7 et recevez cette erreur, mettez à jour pour activer [TLS 1.1 et TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)en tant que protocoles sécurisés par défaut dans WinHTTP dans Windows.</span><span class="sxs-lookup"><span data-stu-id="14887-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="14887-104">Si vous exécutez Windows 10 et que vous recevez une erreur 0x8004de40 avec OneDrive :</span><span class="sxs-lookup"><span data-stu-id="14887-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="14887-105">Redémarrez l’ordinateur affecté lorsque vous êtes connecté à votre domaine Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="14887-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="14887-106">Si un redémarrage ne corrige pas le problème, déjoinez-vous et rejoignez votre appareil à partir d’Azure AD.</span><span class="sxs-lookup"><span data-stu-id="14887-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="14887-107">**Remarque**: vous devez être sur votre réseau d’entreprise lors de ces étapes.</span><span class="sxs-lookup"><span data-stu-id="14887-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="14887-108">N’effectuez pas ces étapes lorsque vous n’êtes pas connecté à votre infrastructure d’entreprise (par exemple, en déplacement).</span><span class="sxs-lookup"><span data-stu-id="14887-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="14887-109">Ouvrez une invite de commandes avec élévation de niveau élevé en sélectionnant **Démarrer,** cliquez avec le bouton droit sur Invite de **commandes,** puis **sélectionnez Exécuter en tant qu’administrateur.**</span><span class="sxs-lookup"><span data-stu-id="14887-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="14887-110">Tapez *dsregcmd /leave et* appuyez sur **Entrée**.</span><span class="sxs-lookup"><span data-stu-id="14887-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="14887-111">Lorsque vous terminez, *tapez dsregcmd /join* et appuyez sur **Entrée**.</span><span class="sxs-lookup"><span data-stu-id="14887-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="14887-112">Lorsque vous terminez, fermez l’invite de commandes.</span><span class="sxs-lookup"><span data-stu-id="14887-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="14887-113">Redémarrez l’ordinateur et connectez-vous à OneDrive.</span><span class="sxs-lookup"><span data-stu-id="14887-113">Reboot the computer, and log into OneDrive.</span></span>