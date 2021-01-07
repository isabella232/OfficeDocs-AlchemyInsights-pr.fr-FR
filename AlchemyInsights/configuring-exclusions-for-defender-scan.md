---
title: Configuration des exclusions pour l’analyse de Microsoft Defender ATP
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
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768402"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="95cf1-102">Configuration des exclusions pour l’analyse de Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="95cf1-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="95cf1-103">En général, vous pouvez exclure certaines extensions de fichier et emplacements de dossier des analyses de Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="95cf1-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="95cf1-104">Vous pouvez également configurer des exclusions pour les fichiers ouverts par certains processus.</span><span class="sxs-lookup"><span data-stu-id="95cf1-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="95cf1-105">Pour plus d’informations, voir [Configurer et valider des exclusions en fonction de l’extension de fichier et de l’emplacement du dossier](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) et [Configurer des exclusions pour les fichiers ouverts par des processus](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="95cf1-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="95cf1-106">Pour configurer des exclusions pour **Windows Server 2016 et 2019**, voir [Configurer les exclusions de l’antivirus Microsoft Defender sur Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="95cf1-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="95cf1-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="95cf1-107">**Mac**</span></span>

<span data-ttu-id="95cf1-108">Pour plus d’informations sur les types d’exclusions pris en charge et la configuration d’une liste d’exclusions pour Mac, voir [Types d’exclusions pris en charge](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) et [Configuration de la liste des exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="95cf1-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="95cf1-109">**Remarque** Vous pouvez également valider les listes d’exclusions à l’aide du fichier de test EICAR.</span><span class="sxs-lookup"><span data-stu-id="95cf1-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="95cf1-110">Pour plus d’informations, voir [Valider les listes d’exclusions à l’aide du fichier de test EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="95cf1-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="95cf1-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="95cf1-111">**Linux**</span></span>

<span data-ttu-id="95cf1-112">Pour plus d’informations sur les types d’exclusions pris en charge et la configuration d’une liste d’exclusions pour Linux, voir [Types d’exclusions pris en charge](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) et [Configurer et valider des exclusions pour Microsoft Defender ATP pour Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="95cf1-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="95cf1-113">**Remarque** Vous pouvez également valider les listes d’exclusions à l’aide du fichier de test EICAR.</span><span class="sxs-lookup"><span data-stu-id="95cf1-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="95cf1-114">Pour plus d’informations, voir [Valider les listes d’exclusions à l’aide du fichier de test EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="95cf1-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 