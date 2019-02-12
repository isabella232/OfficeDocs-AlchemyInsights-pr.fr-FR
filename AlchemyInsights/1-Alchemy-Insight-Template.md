---
title: 'identique au nom de fichier est préférable [règle #-Description]'
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
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939286"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="4fd14-102">Requis Alchemy en-tête H1, H2 ne fonctionnent pas.</span><span class="sxs-lookup"><span data-stu-id="4fd14-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="4fd14-103">Meilleures pratiques et recommandations pour la création de Alchemy :</span><span class="sxs-lookup"><span data-stu-id="4fd14-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="4fd14-p101">**Ne pas imbriquer Alchemy Insights dans les dossiers**- cela interrompt la structure d’url. Nous cherchons à corriger ce.</span><span class="sxs-lookup"><span data-stu-id="4fd14-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="4fd14-106">Fichiers dans le dossier **AlchemyInsights** doivent avoir des ID de la règle et le nom de la règle à partir du [portail partenaires Alchemy](https://alchemyportal.azurewebsites.net) dans le nom de fichier.</span><span class="sxs-lookup"><span data-stu-id="4fd14-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="4fd14-p102">exemple : ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="4fd14-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="4fd14-p103">Utiliser les métadonnées en haut de ce fichier en tant que votre modèle. Rien d’autre n’est nécessaire.</span><span class="sxs-lookup"><span data-stu-id="4fd14-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="4fd14-111">Dans le [portail partenaires Alchemy](https://alchemyportal.azurewebsites.net), naviguez jusqu'à la section **client Insight titre :** et l’utilisation qui en tant que le démarrage d’un point du titre H1 l’aperçu.</span><span class="sxs-lookup"><span data-stu-id="4fd14-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="4fd14-p104">Alchemy Insights doit n'avoir qu’un seul H1 en haut ou erreurs en production. Utilisation de ce **gras** ou autres conventions pour indiquer des sections distinctes ne rendu de H2s.</span><span class="sxs-lookup"><span data-stu-id="4fd14-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="4fd14-114">Ensuite, renseignez le corps du texte à l’aide de la matière brouillon dans la section Détails du client de la page Alchemy règle</span><span class="sxs-lookup"><span data-stu-id="4fd14-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="4fd14-115">Les listes à puces sont correctement</span><span class="sxs-lookup"><span data-stu-id="4fd14-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="4fd14-116">Trop de listes numérotées</span><span class="sxs-lookup"><span data-stu-id="4fd14-116">Numbered lists too</span></span>
    1. <span data-ttu-id="4fd14-117">**Gras** et *italique* sont a-ok</span><span class="sxs-lookup"><span data-stu-id="4fd14-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="4fd14-118">Liens doivent toujours être **« des liens Web » / externe** OR **profond-des liens vers des éléments d’interface utilisateur**, les liens pas internes.</span><span class="sxs-lookup"><span data-stu-id="4fd14-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="4fd14-p105">Et c’est vraiment déjà un peu trop long. Meilleure pratique consiste à environ 400 caractères---</span><span class="sxs-lookup"><span data-stu-id="4fd14-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="4fd14-p106">Une fois votre contenu est prêt, l’extraction vers la branche live. Ensuite, accédez au [portail Alchemy](https://alchemyportal.azurewebsites.net) et entrez le nom de fichier dans le champ url. Assurez-vous que Insight révisé et publié indique « Oui », puis cliquez sur règle de mise à jour. **(Cette recherche plus attrayants dans la nouvelle version du portail - libération bientôt.)** 
 ![champ url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="4fd14-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

