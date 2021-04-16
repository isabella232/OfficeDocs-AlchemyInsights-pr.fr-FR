---
title: Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814262"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="c9e88-102">Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports</span><span class="sxs-lookup"><span data-stu-id="c9e88-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="c9e88-103">**Symptôme**</span><span class="sxs-lookup"><span data-stu-id="c9e88-103">**Symptom**</span></span>

<span data-ttu-id="c9e88-104">Les utilisateurs ne peuvent pas ouvrir les rapports.</span><span class="sxs-lookup"><span data-stu-id="c9e88-104">Users are unable to open reports.</span></span> <span data-ttu-id="c9e88-105">« Une erreur s'est produite.</span><span class="sxs-lookup"><span data-stu-id="c9e88-105">"Something has gone wrong.</span></span> <span data-ttu-id="c9e88-106">Vérifiez les détails techniques pour en savoir plus. »</span><span class="sxs-lookup"><span data-stu-id="c9e88-106">Check technical details for more details."</span></span>

<span data-ttu-id="c9e88-107">**Cause**</span><span class="sxs-lookup"><span data-stu-id="c9e88-107">**Cause**</span></span>

<span data-ttu-id="c9e88-108">Échec de chargement des rapports dans UCI avec l’erreur « Le descripteur de formulaire est null ou n’est pas défini ».</span><span class="sxs-lookup"><span data-stu-id="c9e88-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="c9e88-109">Les rapports dans UCI ont encore besoin de boîtes de dialogue héritées, de sorte que *allowlegacydialogsembedding* doit être activé sur le système du client.</span><span class="sxs-lookup"><span data-stu-id="c9e88-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="c9e88-110">**Solution**</span><span class="sxs-lookup"><span data-stu-id="c9e88-110">**Solution**</span></span>

1. <span data-ttu-id="c9e88-111">Accédez à **Paramètres > Administration > Paramètres système > onglet Général**.</span><span class="sxs-lookup"><span data-stu-id="c9e88-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="c9e88-112">Définissez « Activer l’intégration de certaines boîtes de dialogue héritées dans le client du navigateur Unified Interface » sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="c9e88-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
