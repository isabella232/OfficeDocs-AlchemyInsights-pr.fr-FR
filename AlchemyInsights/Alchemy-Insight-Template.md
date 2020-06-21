---
title: identique au nom de fichier recommandé
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750968"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="1f4fd-102">« En-tête Alchemy obligatoire H1, H2's ne fonctionne pas. »</span><span class="sxs-lookup"><span data-stu-id="1f4fd-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="1f4fd-103">Meilleures pratiques et instructions pour la création de Alchemy :</span><span class="sxs-lookup"><span data-stu-id="1f4fd-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="1f4fd-104">**Ne pas imbriquer les informations Alchemy dans les dossiers**: cette opération va rompre la structure de l’URL.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="1f4fd-105">Nous nous penchons sur cette correction.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="1f4fd-106">Les fichiers dans le dossier **AlchemyInsights** doivent avoir des caractères en minuscules avec des traits d’Union pour les espaces ex.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="1f4fd-107">***procédure d’activation-conservation pour litige***.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="1f4fd-108">Incluez l’ID de la règle ou l’ID du compartiment à partir du [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net) dans le champ ms. Custom.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="1f4fd-109">ex.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-109">ex.</span></span> <span data-ttu-id="1f4fd-110">***ms. Custom : 100021***</span><span class="sxs-lookup"><span data-stu-id="1f4fd-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="1f4fd-111">Utilisez le reste des métadonnées en haut de ce fichier comme modèle.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="1f4fd-112">Dans le [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net), accédez à la section **titre du service client :** et utilisez-la comme point de départ pour votre titre H1 pour la vue d’analyse.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="1f4fd-113">Alchemy Insights ne doit avoir qu’un seul H1 en haut ou ils seront interrompus en production.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="1f4fd-114">H2s ne pas afficher de manière à utiliser le **gras** ou d’autres conventions pour signifier des sections distinctes.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="1f4fd-115">Ensuite, renseignez le corps de texte à l’aide de l’élément brouillon dans la section informations client de la page de la règle Alchemy.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="1f4fd-116">Les listes à puces conviennent parfaitement</span><span class="sxs-lookup"><span data-stu-id="1f4fd-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="1f4fd-117">Listes numérotées</span><span class="sxs-lookup"><span data-stu-id="1f4fd-117">Numbered lists too</span></span>
    1. <span data-ttu-id="1f4fd-118">**Gras** et *italique* sont un-OK</span><span class="sxs-lookup"><span data-stu-id="1f4fd-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="1f4fd-119">Les liens doivent toujours être **« liens vers le Web »/External** ou **des liens détaillés vers les éléments de l’interface utilisateur**, pas les liens internes.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="1f4fd-120">Les images ne sont pas officiellement prises en charge pour le moment, mais elles figurent dans la feuille de route.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="1f4fd-121">Et cela est déjà un peu trop long.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-121">And this is really already a bit too long.</span></span> <span data-ttu-id="1f4fd-122">La meilleure pratique est de 400 caractères---------------------------------</span><span class="sxs-lookup"><span data-stu-id="1f4fd-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="1f4fd-123">Une fois que votre contenu est prêt, tirez-le vers la branche Live.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="1f4fd-124">Ensuite, accédez au [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net) et entrez le nom du fichier dans le champ URL.</span><span class="sxs-lookup"><span data-stu-id="1f4fd-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 