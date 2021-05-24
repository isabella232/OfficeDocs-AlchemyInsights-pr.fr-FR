---
title: Résolution des erreurs de la mise en suspens de la découverte électronique.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583753"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="7d5a5-102">Résolution des erreurs de la mise en suspens de la découverte électronique.</span><span class="sxs-lookup"><span data-stu-id="7d5a5-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="7d5a5-103">Vous rencontrez des problèmes avec les suspensions d'eDiscovery ?</span><span class="sxs-lookup"><span data-stu-id="7d5a5-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="7d5a5-104">Voici quelques bonnes pratiques à prendre en considération :</span><span class="sxs-lookup"><span data-stu-id="7d5a5-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="7d5a5-105">Vérifiez l'état de la distribution des mises en suspens.</span><span class="sxs-lookup"><span data-stu-id="7d5a5-105">Check the hold distribution status.</span></span>  <span data-ttu-id="7d5a5-106">Si l’état est **Activé (en attente)** ou **Désactivé (en attente)**, attendez que la distribution de suspension soit terminée.</span><span class="sxs-lookup"><span data-stu-id="7d5a5-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="7d5a5-107">Fusionnez les mises à jour des suspensions eDiscovery en une seule demande groupée au lieu de mettre à jour la stratégie à plusieurs reprises pour chaque transaction.</span><span class="sxs-lookup"><span data-stu-id="7d5a5-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="7d5a5-108">Exécutez la <policyname> Set-CasePolicy -RetryDistribution dans le Centre de sécurité et conformité PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7d5a5-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="7d5a5-109">Pour plus d’informations, consultez [Se connecter à l’interface PowerShell du Centre de sécurité et conformité](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="7d5a5-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="7d5a5-110">Pour consulter ces paramètres et d’autres meilleures pratiques pour l’atténuation et la résolution des problèmes de mise en suspens de la découverte électronique, consultez [Résoudre les erreurs de mise en suspens de la découverte électronique](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="7d5a5-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="7d5a5-111">Pour plus d’informations sur la résolution d’autres problèmes courants de découverte électronique, consultez [Rechercher, résoudre les problèmes et résoudre de découverte électronique courants](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="7d5a5-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
