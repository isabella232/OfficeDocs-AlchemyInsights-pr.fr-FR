---
title: Problèmes d’accès conditionnel
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013950"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="64d04-102">Problèmes d’accès conditionnel</span><span class="sxs-lookup"><span data-stu-id="64d04-102">Conditional access issues</span></span>

<span data-ttu-id="64d04-103">**Résoudre les problèmes avec le diagnostic de connexion**</span><span class="sxs-lookup"><span data-stu-id="64d04-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="64d04-104">Vous pouvez rapidement découvrir ce qui s’est passé ou diagnostiquer les problèmes liés à la connectez-vous à l’aide du [diagnostic de la sign-in](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="64d04-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="64d04-105">Lancez le diagnostic de connexion.</span><span class="sxs-lookup"><span data-stu-id="64d04-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="64d04-106">Recherchez l’événement à analyser en entrant les détails que vous avez sur l’utilisateur, l’application, l’heure de la signature, l’ID de demande ou l’ID de corrélation.</span><span class="sxs-lookup"><span data-stu-id="64d04-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="64d04-107">Examinez les résultats de diagnostic montrant les détails de ce qui s’est passé et les actions que vous pouvez prendre pour apporter des modifications (si des modifications sont nécessaires).</span><span class="sxs-lookup"><span data-stu-id="64d04-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="64d04-108">**Étapes pour résoudre les problèmes de la sign-in**</span><span class="sxs-lookup"><span data-stu-id="64d04-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="64d04-109">Accédez à la page de signature Azure AD.</span><span class="sxs-lookup"><span data-stu-id="64d04-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="64d04-110">Filtrer les connecteurs par utilisateur, plage de temps, application, état, application cliente, etc.</span><span class="sxs-lookup"><span data-stu-id="64d04-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="64d04-111">Sélectionnez un événement de sign-in et affichez l’onglet Accès conditionnel pour voir quelles stratégies ont été évaluées.</span><span class="sxs-lookup"><span data-stu-id="64d04-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="64d04-112">Cliquez sur la ligne d’une stratégie pour afficher les détails de la stratégie et comprendre pourquoi elle s’est appliquée.</span><span class="sxs-lookup"><span data-stu-id="64d04-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="64d04-113">**Outils permettant de résoudre les problèmes d’une stratégie d’accès conditionnel**</span><span class="sxs-lookup"><span data-stu-id="64d04-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="64d04-114">Le mode Rapport uniquement vous permet d’évaluer une stratégie sans impact sur les utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="64d04-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="64d04-115">L’outil De simulation vous permet de simuler des événements de sign-in et de voir quelles stratégies s’appliquent.</span><span class="sxs-lookup"><span data-stu-id="64d04-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="64d04-116">Le workbook Insights et reporting affiche l’impact en temps réel de chaque stratégie.</span><span class="sxs-lookup"><span data-stu-id="64d04-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="64d04-117">**Stratégies de protection de référence**</span><span class="sxs-lookup"><span data-stu-id="64d04-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="64d04-118">Les stratégies de protection de référence ont été dépréciées.</span><span class="sxs-lookup"><span data-stu-id="64d04-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="64d04-119">Elles ne sont plus appliquées et seront bientôt supprimées du portail Azure.</span><span class="sxs-lookup"><span data-stu-id="64d04-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="64d04-120">Nous vous recommandons d’activer [les paramètres de sécurité par défaut.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="64d04-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="64d04-121">Pour plus d’informations sur l’accès conditionnel, voir :</span><span class="sxs-lookup"><span data-stu-id="64d04-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="64d04-122">[Meilleures pratiques pour l’accès conditionnel dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions de l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Contrôles dans l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Emplacements dans l’accès conditionnel](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="64d04-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
