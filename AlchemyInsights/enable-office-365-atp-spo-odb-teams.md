---
title: Activer la protection avancée contre les menaces Office 365 pour SharePoint, OneDrive et Microsoft teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709905"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2acd0-102">Activer Office 365 protection avancée contre les menaces pour SharePoint Online, OneDrive et Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="2acd0-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="2acd0-103">Accédez à https://protection.office.com et connectez-vous.</span><span class="sxs-lookup"><span data-stu-id="2acd0-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="2acd0-104">Choisissez **Threat management**  >  **Policy**  >  **pièces jointes fiables**pour la stratégie de gestion des menaces.</span><span class="sxs-lookup"><span data-stu-id="2acd0-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="2acd0-105">Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams**, puis cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="2acd0-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="2acd0-106">Recommandation En tant qu’administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** défini sur *true*.</span><span class="sxs-lookup"><span data-stu-id="2acd0-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="2acd0-107">Recommandation [Configurez les alertes](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pour les fichiers détectés.</span><span class="sxs-lookup"><span data-stu-id="2acd0-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="2acd0-108">La fonctionnalité ATP va analyser tous les fichiers dans SharePoint Online, OneDrive ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2acd0-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="2acd0-109">Les fichiers sont analysés de manière asynchrone, via un processus qui utilise des événements d’activité de partage et d’invité, ainsi que des méthodes heuristiques intelligentes et des signaux de menace pour identifier les fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="2acd0-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="2acd0-110">Voir [ATP pour SharePoint, OneDrive et Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2acd0-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>