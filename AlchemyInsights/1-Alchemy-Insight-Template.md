---
title: 'identique au nom de fichier: recommandé [règle #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634502"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="ee5cd-102">En-tête Alchemy obligatoire H1, H2's ne fonctionne pas.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="ee5cd-103">Meilleures pratiques et instructions pour la création de Alchemy:</span><span class="sxs-lookup"><span data-stu-id="ee5cd-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="ee5cd-104">**Ne pas**imbriquer les informations Alchemy dans les dossiers: cette opération va rompre la structure de l'URL.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="ee5cd-105">Nous nous penchons sur cette correction.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="ee5cd-106">Les fichiers dans le dossier **AlchemyInsights** doivent avoir l'ID de règle et le nom de règle du [portail de partenaires Alchemy](https://alchemyportal.azurewebsites.net) dans le nom de fichier.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="ee5cd-107">ex.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-107">ex.</span></span> <span data-ttu-id="ee5cd-108">***976-activer-mettre en attente pour litige***</span><span class="sxs-lookup"><span data-stu-id="ee5cd-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="ee5cd-109">Utilisez les métadonnées en haut de ce fichier comme modèle.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="ee5cd-110">Rien d'autre n'est requis.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-110">Nothing else is required.</span></span>
1. <span data-ttu-id="ee5cd-111">Dans le [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net), accédez à la section **titre du service client:** et utilisez-la comme point de départ pour votre titre H1 pour la vue d'analyse.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="ee5cd-112">Alchemy Insights ne doit avoir qu'un seul H1 en haut ou ils seront interrompus en production.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="ee5cd-113">H2s ne pas afficher de manière à utiliser le **gras** ou d'autres conventions pour signifier des sections distinctes.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="ee5cd-114">Ensuite, renseignez le corps de texte à l'aide de l'élément brouillon dans la section informations client de la page de la règle Alchemy.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="ee5cd-115">Les listes à puces conviennent parfaitement</span><span class="sxs-lookup"><span data-stu-id="ee5cd-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="ee5cd-116">Listes numérotées</span><span class="sxs-lookup"><span data-stu-id="ee5cd-116">Numbered lists too</span></span>
    1. <span data-ttu-id="ee5cd-117">**Gras** et *italique* sont un-OK</span><span class="sxs-lookup"><span data-stu-id="ee5cd-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="ee5cd-118">Les liens doivent toujours être **«liens vers le Web»/External** ou **des liens détaillés vers les éléments de l'interface utilisateur**, pas les liens internes.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="ee5cd-119">Et cela est déjà un peu trop long.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-119">And this is really already a bit too long.</span></span> <span data-ttu-id="ee5cd-120">La meilleure pratique est de 400 caractères---------------------------------</span><span class="sxs-lookup"><span data-stu-id="ee5cd-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="ee5cd-121">Une fois que votre contenu est prêt, tirez-le vers la branche Live.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="ee5cd-122">Ensuite, accédez au [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net) et entrez le nom du fichier dans le champ URL.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="ee5cd-123">Assurez-vous que l'option Aperçu révisé et publié indique «Oui», puis cliquez sur règle de mise à jour.</span><span class="sxs-lookup"><span data-stu-id="ee5cd-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="ee5cd-124">**(Cette Prettier apparaîtra bientôt dans la nouvelle version du portail.)** 
 ![champ URL](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="ee5cd-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

