---
title: Un double-clic sur un fichier Office échoue pour l’ouvrir
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812077"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="0dc43-102">Un double-clic sur un fichier Office échoue pour l’ouvrir</span><span class="sxs-lookup"><span data-stu-id="0dc43-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="0dc43-103">Après avoir double-cliqué sur un fichier Office, vous pouvez voir le programme ouvert, mais le fichier lui-même ne s’ouvre pas.</span><span class="sxs-lookup"><span data-stu-id="0dc43-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="0dc43-104">Ou vous pouvez obtenir l’erreur suivante : « un problème est survenu lors de l’envoi de la commande au programme. »</span><span class="sxs-lookup"><span data-stu-id="0dc43-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="0dc43-105">Il existe de nombreuses causes pour cela, mais les deux solutions les plus courantes sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="0dc43-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="0dc43-106">À partir d’Excel, vérifiez que l’option DDE n’est pas cochée.</span><span class="sxs-lookup"><span data-stu-id="0dc43-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="0dc43-107">L’option peut être trouvée en créant un nouveau classeur, puis en choisissant **options de > de fichiers > avancé**.</span><span class="sxs-lookup"><span data-stu-id="0dc43-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="0dc43-108">Dans la section **général** , désactivez la case à cocher **Ignorer les autres applications qui utilisent l’échange dynamique de données (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="0dc43-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="0dc43-109">Exécutez une réparation en ligne pour restaurer les paramètres par défaut.</span><span class="sxs-lookup"><span data-stu-id="0dc43-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="0dc43-110">Cliquez sur le bouton Démarrer de Windows et recherchez « panneau de configuration ».</span><span class="sxs-lookup"><span data-stu-id="0dc43-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="0dc43-111">Ouvrez le **panneau de configuration**et accédez à **programmes > programmes et fonctionnalités**.</span><span class="sxs-lookup"><span data-stu-id="0dc43-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="0dc43-112">Cliquez ensuite avec le bouton droit sur **Microsoft Office [version]** et choisissez **modifier > réparation en ligne**.</span><span class="sxs-lookup"><span data-stu-id="0dc43-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="0dc43-113">Si aucune de ces solutions ne fonctionne, une liste plus complète de solutions est disponible dans l’article de support technique, un [double-clic sur un fichier Office ne parvient pas à l’ouvrir](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="0dc43-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
