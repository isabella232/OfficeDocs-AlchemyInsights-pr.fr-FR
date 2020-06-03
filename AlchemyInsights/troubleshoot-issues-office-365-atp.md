---
title: Résolution des problèmes liés à la protection avancée contre les menaces Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511110"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="772fd-102">Résolution des problèmes liés à l’ATP Office 365</span><span class="sxs-lookup"><span data-stu-id="772fd-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="772fd-103">**Retards de remise des messages électroniques**?</span><span class="sxs-lookup"><span data-stu-id="772fd-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="772fd-104">Essayez d’utiliser l’option de remise dynamique pour vos stratégies de pièces jointes approuvées ATP.</span><span class="sxs-lookup"><span data-stu-id="772fd-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="772fd-105">Cela permet d’éviter les retards de remise des messages électroniques tout en protégeant les destinataires des fichiers malveillants.</span><span class="sxs-lookup"><span data-stu-id="772fd-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="772fd-106">**Voulez-vous signaler les faux positifs ou les faux négatifs**?</span><span class="sxs-lookup"><span data-stu-id="772fd-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="772fd-107">Utilisez ce lien pour envoyer votre fichier à des fins d’analyse :[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="772fd-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="772fd-108">**Saviez-vous que vous pouvez activer la protection des liens approuvés ATP pour les messages électroniques envoyés entre les personnes de votre organisation**?</span><span class="sxs-lookup"><span data-stu-id="772fd-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="772fd-109">Procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="772fd-109">Follow these steps:</span></span>
    1. <span data-ttu-id="772fd-110">Accédez à https://protection.office.com , puis connectez-vous.</span><span class="sxs-lookup"><span data-stu-id="772fd-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="772fd-111">Accédez à **Threat management**  >  **Policy**  >  **liens fiables**de la stratégie de gestion des menaces.</span><span class="sxs-lookup"><span data-stu-id="772fd-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="772fd-112">Sous **stratégies qui s’appliquent à des destinataires spécifiques**, modifiez (ou ajoutez) une stratégie.</span><span class="sxs-lookup"><span data-stu-id="772fd-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="772fd-113">Sélectionnez **appliquer les liens fiables aux messages envoyés au sein de l’organisation**.</span><span class="sxs-lookup"><span data-stu-id="772fd-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="772fd-114">Enregistrez votre stratégie et laissez environ 30 minutes pour que vos modifications fonctionnent dans votre centre de informations.</span><span class="sxs-lookup"><span data-stu-id="772fd-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="772fd-115">Pour obtenir de l’aide supplémentaire sur la [protection avancée contre les menaces, consultez la rubrique Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="772fd-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>