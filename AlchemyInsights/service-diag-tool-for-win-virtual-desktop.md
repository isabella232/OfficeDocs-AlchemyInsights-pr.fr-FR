---
title: Outil de diagnostic de service pour le bureau virtuel Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665817"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="54ac8-102">Outil de diagnostic de service pour le bureau virtuel Windows</span><span class="sxs-lookup"><span data-stu-id="54ac8-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="54ac8-103">Windows Virtual Desktop (WVD) propose un outil de diagnostic qui permet aux administrateurs d’identifier les erreurs via une seule interface.</span><span class="sxs-lookup"><span data-stu-id="54ac8-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="54ac8-104">Cet outil enregistre les informations relatives aux diagnostics chaque fois que WVD est utilisé par une personne qui a un rôle WVD.</span><span class="sxs-lookup"><span data-stu-id="54ac8-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="54ac8-105">Chaque journal contient des informations sur le rôle WVD impliqué dans l’activité, les messages d’erreur qui s’affichent pendant la session, ainsi que des informations sur le client et l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="54ac8-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="54ac8-106">Azure log Analytics peut être configuré pour capturer le journal d’activité créé par l’outil de diagnostic.</span><span class="sxs-lookup"><span data-stu-id="54ac8-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="54ac8-107">Voici comment procéder :</span><span class="sxs-lookup"><span data-stu-id="54ac8-107">Here's how:</span></span>

1. <span data-ttu-id="54ac8-108">Créez un espace de travail d’analyse des journaux avec le [portail Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ou [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="54ac8-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="54ac8-109">[Connectez les ordinateurs Windows à Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="54ac8-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="54ac8-110">Obtenir l’ID d’espace de travail et la clé primaire de votre espace de travail.</span><span class="sxs-lookup"><span data-stu-id="54ac8-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="54ac8-111">L’Assistant installation a besoin de ces informations pour configurer correctement l’agent et pour s’assurer qu’il peut communiquer avec Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="54ac8-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="54ac8-112">[Transférer les données de diagnostic vers votre espace de travail](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="54ac8-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="54ac8-113">Vous pouvez transférer les données de diagnostic de votre client WVD vers l’analyse du journal pour votre espace de travail.</span><span class="sxs-lookup"><span data-stu-id="54ac8-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="54ac8-114">[Identifier et diagnostiquer les problèmes](https://go.microsoft.com/fwlink/?linkid=2128338) internes ou externes par rapport à WVD.</span><span class="sxs-lookup"><span data-stu-id="54ac8-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="54ac8-115">Pour en savoir plus sur la configuration de l’outil de diagnostic de service pour WVD, consultez [la rubrique use log Analytics for the Diagnostics Feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="54ac8-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
