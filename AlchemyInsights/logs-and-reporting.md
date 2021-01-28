---
title: Journaux et rapports
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031498"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="f3606-102">Journaux et rapports</span><span class="sxs-lookup"><span data-stu-id="f3606-102">Logs and Reporting</span></span>

<span data-ttu-id="f3606-103">[Le FAQ sur les rapports Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) répond aux questions fréquemment posées sur la création de rapports Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f3606-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="f3606-104">Pour plus d’informations, [voir rapports Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="f3606-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="f3606-105">**Résolution des problèmes avec Audit**</span><span class="sxs-lookup"><span data-stu-id="f3606-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="f3606-106">Si vous avez des problèmes à voir certaines activités d’audit et que l’activité manquante figure dans cette [liste,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)veuillez déposer un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="f3606-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="f3606-107">Si vous avez des problèmes à voir les journaux d’audit dans votre client, déposez un ticket de support.</span><span class="sxs-lookup"><span data-stu-id="f3606-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="f3606-108">Si vos activités d’audit ne s’affichent pas immédiatement dans le portail Azure, consultez nos informations de [latence](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) et déposez un ticket de support si le délai dépasse la latence documentée.</span><span class="sxs-lookup"><span data-stu-id="f3606-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="f3606-109">Rétention des journaux d’activité Azure AD</span><span class="sxs-lookup"><span data-stu-id="f3606-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="f3606-110">Si vous ne voyez pas l’audit de la plage de dates que vous avez sélectionnée, vous pouvez télécharger jusqu’à 250 000 lignes (triées par rapport aux plus récentes) de signatures à partir du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="f3606-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="f3606-111">Pour plus d’informations, [voir téléchargement des activités d’audit.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="f3606-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="f3606-112">**Résolution des problèmes avec les sign-ins**</span><span class="sxs-lookup"><span data-stu-id="f3606-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="f3606-113">Vous pouvez uniquement voir les 30 derniers jours de données si vous avez une licence Azure AD Premium (P1 ou P2) pour votre client.</span><span class="sxs-lookup"><span data-stu-id="f3606-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="f3606-114">Les connecteurs sont disponibles uniquement pour les locataires Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="f3606-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="f3606-115">Il n’est pas disponible pour les locataires avec licence gratuite ou de base.</span><span class="sxs-lookup"><span data-stu-id="f3606-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="f3606-116">Si votre client dispose d’une licence Premium P1 et que vous ne pouvez pas voir les inscriptions, consultez nos informations de [latence](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) et déposez un ticket de support si le délai dépasse la latence documentée.</span><span class="sxs-lookup"><span data-stu-id="f3606-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="f3606-117">Si vous ne voyez pas toutes les informations de la plage de dates sélectionnée, notez que vous pouvez télécharger jusqu’à 250 000 lignes (triées par date la plus récente) de signatures à partir du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="f3606-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="f3606-118">Pour plus d’informations, voir téléchargement des activités [de signature.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="f3606-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="f3606-119">**Résoudre les problèmes de rapports de sécurité (utilisateurs signalés à risque, se connectant à risque)**</span><span class="sxs-lookup"><span data-stu-id="f3606-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="f3606-120">Utilisateurs marqués pour le rapport de sécurité des risques</span><span class="sxs-lookup"><span data-stu-id="f3606-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="f3606-121">Rapport sur les sign-ins à risque dans le portail Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f3606-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="f3606-122">Événements à risque Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f3606-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
