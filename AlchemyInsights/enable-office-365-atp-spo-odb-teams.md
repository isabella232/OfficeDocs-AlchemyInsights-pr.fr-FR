---
title: Activer la protection avancée contre les menaces Office 365 pour SharePoint, OneDrive et Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403031"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="7b773-102">Activer Office 365 protection avancée contre les menaces pour SharePoint Online, OneDrive et Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="7b773-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="7b773-103">Accédez à https://protection.office.com et connectez-vous.</span><span class="sxs-lookup"><span data-stu-id="7b773-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="7b773-104">Choisissez**pièces jointes fiables**pour la**stratégie** > de **gestion** > des menaces.</span><span class="sxs-lookup"><span data-stu-id="7b773-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="7b773-105">Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams**, puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="7b773-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="7b773-106">Recommandation En tant qu'administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** défini sur *true*.</span><span class="sxs-lookup"><span data-stu-id="7b773-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="7b773-107">Recommandation [Configurez les alertes](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pour les fichiers détectés.</span><span class="sxs-lookup"><span data-stu-id="7b773-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="7b773-108">La fonctionnalité ATP va analyser tous les fichiers dans SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7b773-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="7b773-109">Les fichiers sont analysés de manière asynchrone, via un processus qui utilise des événements d'activité de partage et d'invité, ainsi que des méthodes heuristiques intelligentes et des signaux de menace pour identifier les fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="7b773-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="7b773-110">Voir [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams) (en anglais).</span><span class="sxs-lookup"><span data-stu-id="7b773-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>