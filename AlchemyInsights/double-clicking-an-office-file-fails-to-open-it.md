---
title: Le double-clic sur un fichier Office ne parvient pas à l'ouvrir
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814803"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="93524-102">Le double-clic sur un fichier Office ne parvient pas à l'ouvrir</span><span class="sxs-lookup"><span data-stu-id="93524-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="93524-103">Après avoir double-cliqué sur un fichier Office, le programme peut s'ouvrir, mais le fichier proprement dit ne s'ouvre pas.</span><span class="sxs-lookup"><span data-stu-id="93524-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="93524-104">Sinon, vous pouvez obtenir l'erreur : « Un problème s'est produite lors de l'envoi de la commande au programme. »</span><span class="sxs-lookup"><span data-stu-id="93524-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="93524-105">Il existe de nombreuses causes à cela, mais les deux solutions les plus courantes sont :</span><span class="sxs-lookup"><span data-stu-id="93524-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="93524-106">Dans Excel, assurez-vous que l'option DDE est désactivée.</span><span class="sxs-lookup"><span data-stu-id="93524-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="93524-107">L'option est disponible en créant un classez, puis en choisissant > Options > **Avancé**.</span><span class="sxs-lookup"><span data-stu-id="93524-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="93524-108">Dans la section **Général,** décochez la section Ignorer les autres applications qui utilisent **Dynamic Data Exchange (DDE).**</span><span class="sxs-lookup"><span data-stu-id="93524-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="93524-109">Exécutez une réparation en ligne pour restaurer les paramètres par défaut.</span><span class="sxs-lookup"><span data-stu-id="93524-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="93524-110">Cliquez sur le bouton Démarrer de Windows et recherchez « Panneau de contrôle ».</span><span class="sxs-lookup"><span data-stu-id="93524-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="93524-111">Ouvrez **le Panneau de** contrôle et allez à Programmes > programmes et **fonctionnalités.**</span><span class="sxs-lookup"><span data-stu-id="93524-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="93524-112">Cliquez ensuite avec le **bouton droit Microsoft Office [Version]** et choisissez **Modifier > Réparation en ligne.**</span><span class="sxs-lookup"><span data-stu-id="93524-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="93524-113">Si aucune de ces solutions ne fonctionne, une liste plus complète de solutions est trouvée dans l'article de support, le double-clic sur un fichier Office ne [parvient pas à l'ouvrir.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="93524-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
