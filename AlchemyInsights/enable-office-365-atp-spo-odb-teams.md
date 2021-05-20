---
title: Activer Office 365 atp pour SharePoint, OneDrive et Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543926"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c1ad6-102">Activez Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive et Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c1ad6-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c1ad6-103">Accédez à https://protection.office.com et connectez-vous.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c1ad6-104">Choose **Threat management**  >  **Policy** Safe  >  **Attachments**.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c1ad6-105">Sélectionnez **Activer Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams,** puis cliquez sur **Enregistrer.**</span><span class="sxs-lookup"><span data-stu-id="c1ad6-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c1ad6-106">(Recommandé) En tant qu’administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** définie sur *true*.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c1ad6-107">(Recommandé) [Configurer des alertes pour](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) les fichiers détectés.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c1ad6-108">Microsoft Defender pour Office 365 n’analyse pas chaque fichier dans SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c1ad6-109">Les fichiers sont analysés de manière asynchrone, par le biais d’un processus qui utilise des événements de partage et d’activité invité, ainsi que des signaux heuristiques intelligents et des signaux de menace pour identifier les fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="c1ad6-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c1ad6-110">Consultez [Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c1ad6-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>