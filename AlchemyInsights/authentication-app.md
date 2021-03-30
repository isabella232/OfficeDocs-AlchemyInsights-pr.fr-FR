---
title: Application d’authentification
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403800"
---
# <a name="authentication-app"></a><span data-ttu-id="5f511-102">Application d’authentification</span><span class="sxs-lookup"><span data-stu-id="5f511-102">Authentication app</span></span>

<span data-ttu-id="5f511-103">Si vous êtes un administrateur général, vous pouvez rapidement découvrir ce qui s’est passé ou diagnostiquer les problèmes liés à la connectez-vous à l’aide des [diagnostics de la signature.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="5f511-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="5f511-104">Démarrez les diagnostics en cliquant sur le bouton «[Lancer le diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)».</span><span class="sxs-lookup"><span data-stu-id="5f511-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="5f511-105">Recherchez l’événement à analyser en entrant les détails que vous avez sur l’utilisateur, l’application, l’heure de la signature, l’ID de demande ou l’ID de corrélation.</span><span class="sxs-lookup"><span data-stu-id="5f511-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="5f511-106">Examinez les résultats du diagnostic. Ils vous indiqueront ce qui s’est produit et les actions que vous pouvez prendre pour apporter des modifications, en cas de besoin.</span><span class="sxs-lookup"><span data-stu-id="5f511-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="5f511-107">**Vérifiez le scénario applicable :**</span><span class="sxs-lookup"><span data-stu-id="5f511-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="5f511-108">Si un utilisateur ne fait pas l’objet d’une notification Push dans l’application Microsoft Authenticator, vérifiez qu’il n’est pas affiché sous l’authentification MFA bloquée, comme décrit dans Bloquer et débloquer les [utilisateurs.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="5f511-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="5f511-109">Si l’utilisateur n’est pas bloqué pour l’authentification MFA mais ne reçoit pas de notification Push, il peut ouvrir l’application Microsoft Authenticator, qui tirera les demandes d’approbation en attente.</span><span class="sxs-lookup"><span data-stu-id="5f511-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="5f511-110">En tant qu’autre méthode de sign-in, l’utilisateur peut également cliquer sur Sign in another way et choisir d’utiliser un code de vérification à partir de mon application mobile.</span><span class="sxs-lookup"><span data-stu-id="5f511-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="5f511-111">L’application Microsoft Authenticator est la seule méthode disponible pour de nombreux utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="5f511-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="5f511-112">[En savoir plus sur les paramètres de sécurité par défaut,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)consultez le FAQ de l’application [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) pour connaître les questions fréquemment posées et la façon de les résoudre.</span><span class="sxs-lookup"><span data-stu-id="5f511-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="5f511-113">**Vidéos recommandées**</span><span class="sxs-lookup"><span data-stu-id="5f511-113">**Recommended Videos**</span></span>

<span data-ttu-id="5f511-114">[Comment configurer l’application Authenticator sur un nouveau téléphone (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="5f511-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
