---
title: 1490-dépannage-échecs de découverte électronique
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277837"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="cbb0f-102">Résoudre les erreurs de recherche de contenu</span><span class="sxs-lookup"><span data-stu-id="cbb0f-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="cbb0f-103">Rencontrez-vous des problèmes avec la recherche de contenu ou lorsque vous exportez des résultats de recherche ?</span><span class="sxs-lookup"><span data-stu-id="cbb0f-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="cbb0f-104">Par exemple, avez-vous reçu les informations suivantes lors de l’exécution des recherches ?</span><span class="sxs-lookup"><span data-stu-id="cbb0f-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="cbb0f-105">Erreurs CS008 ou CS012</span><span class="sxs-lookup"><span data-stu-id="cbb0f-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="cbb0f-106">Erreurs d’occupation/de délai d’attente du serveur</span><span class="sxs-lookup"><span data-stu-id="cbb0f-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="cbb0f-107">Une erreur d’application s’est produite</span><span class="sxs-lookup"><span data-stu-id="cbb0f-107">Application error occurred</span></span>

<span data-ttu-id="cbb0f-108">Ou lorsque vous recherchez ou exportez des résultats à partir d’un grand nombre de boîtes aux lettres (plus de 100 000 boîtes aux lettres), recevez-vous des erreurs d’exportation ?</span><span class="sxs-lookup"><span data-stu-id="cbb0f-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="cbb0f-109">Pour ces types d’erreurs, essayez de relancer la recherche pour les emplacements de contenu ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="cbb0f-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="cbb0f-110">Pour plus d’informations, consultez  [cet article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="cbb0f-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="cbb0f-111">Si vous exportez plus de 100 000 boîtes aux lettres, vous devez utiliser le PowerShell suivant pour télécharger les résultats de l’exportation :  [Exporter les résultats de plus de 100 000 boîtes aux lettres](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="cbb0f-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
