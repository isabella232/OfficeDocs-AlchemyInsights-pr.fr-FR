---
title: Les indicateurs ne fonctionnent pas à l’aide du navigateur Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651489"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="5bbdc-102">Les indicateurs ne fonctionnent pas à l’aide du navigateur Edge</span><span class="sxs-lookup"><span data-stu-id="5bbdc-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="5bbdc-103">Une fois que vous avez créé un indicateur, il n'est pas reconnu par Edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="5bbdc-104">Pour plus d’informations, consultez [Créer des indicateurs pour les IP et URL/domaines](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="5bbdc-105">Étape 1 : vérifier les éléments suivants</span><span class="sxs-lookup"><span data-stu-id="5bbdc-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="5bbdc-106">Vérifiez que l’indicateur est correct (aucune faute de frappe dans IP/URL, action correcte, groupes RBAC corrects).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="5bbdc-107">Attendez au minimum 2 heures après la création de l'indicateur pour tenir compte d'une éventuelle latence.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="5bbdc-108">Confirmez que le ou les systèmes sont intégrés à Microsoft Defender pour point de terminaison.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="5bbdc-109">Vérifiez que le ou les systèmes peuvent communiquer avec le cloud.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="5bbdc-110">Vérifiez que Smartscreen est activé et accessible en accédant au [site de test](https://demo.smartscreen.msft.net).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="5bbdc-111">Étape 2 : résoudre le problème potentiel</span><span class="sxs-lookup"><span data-stu-id="5bbdc-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="5bbdc-112">Assurez-vous que le client répond aux exigences.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="5bbdc-113">Pour plus d’informations, consultez [Créer des indicateurs pour les IP et URL/domaines](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="5bbdc-114">Assurez-vous que vous exécutez la dernière version du navigateur Edge.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="5bbdc-115">Pour connaître la dernière version, consultez [Découvrez la version de Microsoft Edge que vous avez](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="5bbdc-116">Redémarrez le navigateur Edge.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="5bbdc-117">Accédez au site pour lequel vous avez configuré un indicateur.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="5bbdc-118">Si le site n’apparaît pas comme prévu, passez à l’étape 3.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="5bbdc-119">Étape 3 : collecter les données</span><span class="sxs-lookup"><span data-stu-id="5bbdc-119">Step 3: Collect data</span></span>

- <span data-ttu-id="5bbdc-120">Collectez les données de diagnostic **MDEClientAnalyzer**.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="5bbdc-121">Pour obtenir des instructions, consultez [Problèmes avec les ordinateurs d’intégration à Microsoft Defender pour point de terminaison](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="5bbdc-122">Si vous êtes à l’aise avec l’installation et la collecte d’une trace Fiddler, consultez [Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="5bbdc-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="5bbdc-123">Si vous préférez obtenir des conseils à partir de Support Microsoft, sélectionnez l’icône Support ci-dessous pour ouvrir un cas de support.</span><span class="sxs-lookup"><span data-stu-id="5bbdc-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
