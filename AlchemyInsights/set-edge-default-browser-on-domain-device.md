---
title: Définir Microsoft Edge comme navigateur par défaut sur un appareil joint à un domaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426839"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="477fe-102">Définir Microsoft Edge comme navigateur par défaut sur un appareil joint à un domaine</span><span class="sxs-lookup"><span data-stu-id="477fe-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="477fe-103">Définir Microsoft Edge comme navigateur par défaut :</span><span class="sxs-lookup"><span data-stu-id="477fe-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="477fe-104">[Créez un fichier de configuration d’associations par défaut](https://go.microsoft.com/fwlink/?linkid=2132437) et stockez-le localement ou sur un partage réseau.</span><span class="sxs-lookup"><span data-stu-id="477fe-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="477fe-105">Ouvrez l’éditeur de stratégies de groupe, puis accédez à **Configuration d’un ordinateur** > **Modèlesodèles d’administration** > **Composants Windows** > **Explorateur de fichiers**.</span><span class="sxs-lookup"><span data-stu-id="477fe-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="477fe-106">Sélectionnez **Définir un fichier de configuration d’associations par défaut**.</span><span class="sxs-lookup"><span data-stu-id="477fe-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="477fe-107">Sélectionnez **Paramètre de stratégie**, puis sélectionnez **Activé**.</span><span class="sxs-lookup"><span data-stu-id="477fe-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="477fe-108">Sous **options**, entrez l’emplacement de votre fichier de configuration d’associations par défaut, puis sélectionnez **OK**.</span><span class="sxs-lookup"><span data-stu-id="477fe-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
