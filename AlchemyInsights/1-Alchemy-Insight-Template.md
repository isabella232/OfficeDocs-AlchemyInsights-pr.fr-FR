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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>En-tête Alchemy obligatoire H1, H2's ne fonctionne pas.
Meilleures pratiques et instructions pour la création de Alchemy:

1. **Ne pas**imbriquer les informations Alchemy dans les dossiers: cette opération va rompre la structure de l'URL. Nous nous penchons sur cette correction.
1. Les fichiers dans le dossier **AlchemyInsights** doivent avoir l'ID de règle et le nom de règle du [portail de partenaires Alchemy](https://alchemyportal.azurewebsites.net) dans le nom de fichier.
    1. ex. ***976-activer-mettre en attente pour litige***
1. Utilisez les métadonnées en haut de ce fichier comme modèle. Rien d'autre n'est requis.
1. Dans le [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net), accédez à la section **titre du service client:** et utilisez-la comme point de départ pour votre titre H1 pour la vue d'analyse. 
    > [!NOTE]
    > Alchemy Insights ne doit avoir qu'un seul H1 en haut ou ils seront interrompus en production. H2s ne pas afficher de manière à utiliser le **gras** ou d'autres conventions pour signifier des sections distinctes.
1. Ensuite, renseignez le corps de texte à l'aide de l'élément brouillon dans la section informations client de la page de la règle Alchemy.
    1. Les listes à puces conviennent parfaitement
    1. Listes numérotées
    1. **Gras** et *italique* sont un-OK
    1. Les liens doivent toujours être **«liens vers le Web»/External** ou **des liens détaillés vers les éléments de l'interface utilisateur**, pas les liens internes.

Et cela est déjà un peu trop long. La meilleure pratique est de 400 caractères---------------------------------

Une fois que votre contenu est prêt, tirez-le vers la branche Live. Ensuite, accédez au [portail du partenaire Alchemy](https://alchemyportal.azurewebsites.net) et entrez le nom du fichier dans le champ URL. Assurez-vous que l'option Aperçu révisé et publié indique «Oui», puis cliquez sur règle de mise à jour. **(Cette Prettier apparaîtra bientôt dans la nouvelle version du portail.)** 
 ![champ URL](media/for-content-team.PNG)

