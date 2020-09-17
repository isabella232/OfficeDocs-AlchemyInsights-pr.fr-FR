---
title: Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806433"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="2f835-102">Activer l’incorporation de boîtes de dialogue héritées pour ouvrir les rapports</span><span class="sxs-lookup"><span data-stu-id="2f835-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="2f835-103">**Symptôme**</span><span class="sxs-lookup"><span data-stu-id="2f835-103">**Symptom**</span></span>

<span data-ttu-id="2f835-104">Les utilisateurs ne peuvent pas ouvrir les rapports.</span><span class="sxs-lookup"><span data-stu-id="2f835-104">Users are unable to open reports.</span></span> <span data-ttu-id="2f835-105">« Une erreur s'est produite.</span><span class="sxs-lookup"><span data-stu-id="2f835-105">"Something has gone wrong.</span></span> <span data-ttu-id="2f835-106">Vérifiez les détails techniques pour en savoir plus. »</span><span class="sxs-lookup"><span data-stu-id="2f835-106">Check technical details for more details."</span></span>

<span data-ttu-id="2f835-107">**Cause**</span><span class="sxs-lookup"><span data-stu-id="2f835-107">**Cause**</span></span>

<span data-ttu-id="2f835-108">Échec de chargement des rapports dans UCI avec l’erreur « Le descripteur de formulaire est null ou n’est pas défini ».</span><span class="sxs-lookup"><span data-stu-id="2f835-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="2f835-109">Les rapports dans UCI ont encore besoin de boîtes de dialogue héritées, de sorte que *allowlegacydialogsembedding* doit être activé sur le système du client.</span><span class="sxs-lookup"><span data-stu-id="2f835-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="2f835-110">**Solution**</span><span class="sxs-lookup"><span data-stu-id="2f835-110">**Solution**</span></span>

1. <span data-ttu-id="2f835-111">Accédez à **Paramètres > Administration > Paramètres système > onglet Général**.</span><span class="sxs-lookup"><span data-stu-id="2f835-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="2f835-112">Définissez « Activer l’intégration de certaines boîtes de dialogue héritées dans le client du navigateur Unified Interface » sur **Oui**.</span><span class="sxs-lookup"><span data-stu-id="2f835-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
