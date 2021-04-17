---
title: L’icône de calendrier n’apparaît pas dans le client Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819951"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="fee11-102">L’icône de calendrier n’apparaît pas dans le client Teams</span><span class="sxs-lookup"><span data-stu-id="fee11-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="fee11-103">L’onglet Calendrier dans Teams nécessite l’accès à une boîte aux lettres Exchange par l’entremise des Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fee11-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="fee11-104">La boîte aux lettres Exchange peut être en ligne ou en local.</span><span class="sxs-lookup"><span data-stu-id="fee11-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="fee11-105">Pour les utilisateurs en ligne ne disposant pas de l’onglet Calendrier, assurez-vous qu’ils [sont titulaires d’une licence pour une boîte aux lettres Exchange Online et que la boîte aux lettres est activée](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="fee11-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="fee11-106">Si l’utilisateur dispose d’une boîte aux lettres valide dans Exchange Online, mais ne peut pas consulter l’onglet Calendrier, il est possible que vous rencontriez un problème de réseau.</span><span class="sxs-lookup"><span data-stu-id="fee11-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="fee11-107">Utilisez l’ [Analyseur de connectivité à distance Microsoft](https://testconnectivity.microsoft.com/) et exécutez les **tests de connectivité des services Web Microsoft Exchange** pour l’utilisateur concerné.</span><span class="sxs-lookup"><span data-stu-id="fee11-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="fee11-108">Activez la case à cocher [Applications Teams - stratégies de configuration pour l’application](https://admin.teams.microsoft.com/policies/app-setup) Pour vérifier que l’application calendrier n’a pas été supprimée de la stratégie appliquée à l’utilisateur (il s’agit probablement de **Global (par défaut à l’échelle de l’organisation)**.</span><span class="sxs-lookup"><span data-stu-id="fee11-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="fee11-109">Si vos utilisateurs sont hébergés en local, vous devez vérifier que votre configuration hybride est saine.</span><span class="sxs-lookup"><span data-stu-id="fee11-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="fee11-110">Utilisez l’ [Assistant configuration hybride](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) pour résoudre les problèmes.</span><span class="sxs-lookup"><span data-stu-id="fee11-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="fee11-111">Notez que [Teams nécessite Exchange 2016 CU3 ou une version ultérieure](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="fee11-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
