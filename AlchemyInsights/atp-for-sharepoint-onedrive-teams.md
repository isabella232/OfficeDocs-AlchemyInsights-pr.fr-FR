---
title: PACM pour SharePoint, OneDrive et Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715559"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a24d3-102">PACM pour SharePoint, OneDrive et Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a24d3-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a24d3-103">Procédez comme suit pour activer la protection avancée contre les menaces :</span><span class="sxs-lookup"><span data-stu-id="a24d3-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="a24d3-104">Accédez à [https://protection.office.com](https://protection.office.com) et connectez-vous à l’aide d’un compte d’administrateur général ou d’administrateur de sécurité.</span><span class="sxs-lookup"><span data-stu-id="a24d3-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a24d3-105">Dans le volet de navigation de gauche, sous **gestion des menaces**, sélectionnez **stratégie** de \> **pièces jointes fiables**.</span><span class="sxs-lookup"><span data-stu-id="a24d3-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a24d3-106">Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="a24d3-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a24d3-107">[Créer une stratégie d’alerte d’activité](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) pour recevoir des notifications lors de la détection de fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="a24d3-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a24d3-108">Pour obtenir des instructions complètes, consultez cette [rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a24d3-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a24d3-109">**Remarque**: par conception, la protection avancée contre les menaces n’analyse pas tous les fichiers dans SharePoint Online, OneDrive entreprise ou Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a24d3-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a24d3-110">Les fichiers sont analysés de manière asynchrone par un processus qui utilise l’activité de partage, l’activité des invités et des signaux de menace pour identifier les fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="a24d3-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a24d3-111">Pour plus d’informations, consultez cette [rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a24d3-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
