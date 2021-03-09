---
title: Configurer et valider des exclusions pour MDATP sur un ordinateur Linux
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568618"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="e3dfb-102">Configurer et valider des exclusions pour MDATP sur un ordinateur Linux</span><span class="sxs-lookup"><span data-stu-id="e3dfb-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="e3dfb-103">Vous pouvez exclure certains fichiers, dossiers, processus et fichiers ouverts par processus des analyses MDATP.</span><span class="sxs-lookup"><span data-stu-id="e3dfb-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="e3dfb-104">Les exclusions permettent d’éviter une détection incorrecte des logiciels et des fichiers uniques ou personnalisés pour votre organisation.</span><span class="sxs-lookup"><span data-stu-id="e3dfb-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="e3dfb-105">Les exclusions contribuent également à atténuer les problèmes de performances causés par MDATP.</span><span class="sxs-lookup"><span data-stu-id="e3dfb-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="e3dfb-106">Pour plus d’informations, voir Configurer et valider des [exclusions pour MDATP pour Linux.](https://go.microsoft.com/fwlink/?linkid=2144517)</span><span class="sxs-lookup"><span data-stu-id="e3dfb-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e3dfb-107">Les exclusions décrites dans cet article ne s’appliquent pas aux autres fonctionnalités de MDATP pour Linux, notamment la détection et la réponse des points de terminaison (EDR).</span><span class="sxs-lookup"><span data-stu-id="e3dfb-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="e3dfb-108">Les fichiers que vous excluez à l’aide des méthodes décrites dans cet article peuvent toujours déclencher des alertes EDR et d’autres fonctionnalités de détection.</span><span class="sxs-lookup"><span data-stu-id="e3dfb-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
