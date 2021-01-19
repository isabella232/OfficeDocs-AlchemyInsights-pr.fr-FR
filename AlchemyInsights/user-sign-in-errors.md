---
title: Erreurs de connexion d’un utilisateur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886794"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="d88ed-102">Erreurs de connexion d’un utilisateur</span><span class="sxs-lookup"><span data-stu-id="d88ed-102">User sign-in errors</span></span>

<span data-ttu-id="d88ed-103">**Résoudre les problèmes avec le diagnostic de connexion**</span><span class="sxs-lookup"><span data-stu-id="d88ed-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="d88ed-104">Pour détecter la cause ou diagnostiquer les problèmes liés à la connexion de l’utilisateur, effectuez ces étapes :</span><span class="sxs-lookup"><span data-stu-id="d88ed-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="d88ed-105">Lancez le [diagnostic de connexion](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="d88ed-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="d88ed-106">Recherchez l’événement à analyser en entrant les détails dont vous avez besoin sur l’utilisateur, l’application, l’heure de la connexion, l’ID de demande ou l’ID de corrélation.</span><span class="sxs-lookup"><span data-stu-id="d88ed-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="d88ed-107">Examinez les résultats de diagnostic en indiquant les détails de ce qui s’est produit et les actions que vous pouvez prendre pour apporter des modifications, si des modifications sont nécessaires.</span><span class="sxs-lookup"><span data-stu-id="d88ed-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="d88ed-108">**Recherchez-vous des informations sur les codes d’erreur AADSTS renvoyés à partir du service de jeton de sécurité Azure Active Directory (Azure AD) ?**</span><span class="sxs-lookup"><span data-stu-id="d88ed-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="d88ed-109">Lisez [cet article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) pour trouver des descriptions  d’erreurs AADSTS, des correctifs et quelques solutions de contournement suggérées</span><span class="sxs-lookup"><span data-stu-id="d88ed-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>