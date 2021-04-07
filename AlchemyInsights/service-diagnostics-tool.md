---
title: Outil de diagnostic de service pour Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590277"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="f2162-102">Outil de diagnostic de service pour Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="f2162-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="f2162-103">Windows Virtual Desktop (WVD) offre un outil de diagnostic qui permet aux administrateurs d'identifier les erreurs par le biais d'une interface unique.</span><span class="sxs-lookup"><span data-stu-id="f2162-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="f2162-104">Cet outil enregistre les informations relatives aux diagnostics chaque fois que l' UDS est utilisé par une personne à laquelle un rôle UDS a été attribué.</span><span class="sxs-lookup"><span data-stu-id="f2162-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="f2162-105">Chaque journal contient des informations sur le rôle de l'UVE impliqué dans l'activité, les messages d'erreur qui apparaissent pendant la session, ainsi que des informations sur le locataire et l'utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f2162-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="f2162-106">Les analyses de journaux Azure peuvent être configurées pour capturer le journal d'activité créé par l'outil de diagnostic en suivant ces étapes :</span><span class="sxs-lookup"><span data-stu-id="f2162-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="f2162-107">Créez un espace de travail pour les analyses de journaux avec le [portail Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="f2162-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="f2162-108">[Connecter les ordinateurs Windows à Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="f2162-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="f2162-109">Obtenez l'ID de l'espace de travail et la clé primaire de votre espace de travail.</span><span class="sxs-lookup"><span data-stu-id="f2162-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="f2162-110">L'assistant d'installation a besoin de ces informations pour configurer correctement l'agent et s'assurer qu'il peut communiquer avec Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="f2162-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="f2162-111">[Transférez les données de diagnostic dans votre espace de travail](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="f2162-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="f2162-112">Vous pouvez pousser les données de diagnostic de votre locataire WVD vers les analyses de journaux de votre espace de travail.</span><span class="sxs-lookup"><span data-stu-id="f2162-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="f2162-113">[Identifier et diagnostiquer ](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)les problèmes internes ou externes liés à la DVG.</span><span class="sxs-lookup"><span data-stu-id="f2162-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="f2162-114">Pour en savoir plus sur la configuration de l'outil de diagnostic de service pour WVD, voir Utiliser l'analyse des journaux pour la fonction de diagnostic.</span><span class="sxs-lookup"><span data-stu-id="f2162-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>