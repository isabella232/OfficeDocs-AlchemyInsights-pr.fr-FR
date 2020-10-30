---
title: Dépannage de Microsoft Defender pour Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801441"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="a65af-102">Dépannage de Microsoft Defender pour Office 365</span><span class="sxs-lookup"><span data-stu-id="a65af-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="a65af-103">Remarquez-vous des retards dans la remise des messages ?</span><span class="sxs-lookup"><span data-stu-id="a65af-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="a65af-104">Utilisez l’option de [remise dynamique](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dans votre stratégie de pièces jointes approuvées ATP.</span><span class="sxs-lookup"><span data-stu-id="a65af-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="a65af-105">Cela permet d’éviter les retards de message tout en protégeant les destinataires des fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="a65af-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="a65af-106">Voulez-vous signaler les faux positifs ou les faux négatifs à Microsoft ?</span><span class="sxs-lookup"><span data-stu-id="a65af-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="a65af-107">Utilisez ce [lien](https://www.microsoft.com/wdsi/filesubmission/) pour soumettre des fichiers pour analyse.</span><span class="sxs-lookup"><span data-stu-id="a65af-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="a65af-108">Saviez-vous que vous pouvez activer la protection des liens fiables pour les messages internes envoyés entre les destinataires au sein de votre organisation ?</span><span class="sxs-lookup"><span data-stu-id="a65af-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="a65af-109">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="a65af-109">Follow these steps:</span></span>

  1. <span data-ttu-id="a65af-110">Accédez à [https://protection.office.com](https://protection.office.com) et connectez-vous à l’aide d’un compte d’administrateur général ou d’administrateur de sécurité.</span><span class="sxs-lookup"><span data-stu-id="a65af-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="a65af-111">Dans le volet de navigation de gauche, sous **gestion des menaces** , sélectionnez **Policy** \> **liens approuvés** de stratégie.</span><span class="sxs-lookup"><span data-stu-id="a65af-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="a65af-112">Dans la section **stratégies qui s’appliquent à l’ensemble de l’organisation** , sélectionnez la stratégie, puis cliquez sur **modifier** .</span><span class="sxs-lookup"><span data-stu-id="a65af-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="a65af-113">Sous **paramètres** , activez l' **application de liens fiables aux messages envoyés au sein de l’organisation** .</span><span class="sxs-lookup"><span data-stu-id="a65af-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
