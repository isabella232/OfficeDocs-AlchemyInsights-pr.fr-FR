---
title: le même nom de fichier est préférable
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312823"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>« En-tête Alchemy obligatoire H1, les H2 ne fonctionnent pas. »
Meilleures pratiques et instructions pour la authory Alchemy :

1. **N’imbriez pas** les Informations alchemin dans les dossiers , ce qui va rompre la structure de l’URL. Nous cherchons à résoudre ce problème.
1. Les fichiers **du dossier AlchemyInsights** doivent avoir des noms de fichiers minuscules avec des tirets pour les espaces ex. **_procédure d’activer-la-attente pour litige._**
    1. Incluez l’ID de règle ou l’ID de compartiment du portail [Partenaire Alchemy](https://alchemyportal.azurewebsites.net) dans le champ ms.custom. ex. ***ms.custom: 100021***
1. Utilisez le reste des métadonnées en haut de ce fichier comme modèle.
1. Dans le [portail partenaire Alchemy,](https://alchemyportal.azurewebsites.net)accédez à la section **Titre** de l’insight client : et utilisez-le comme point de départ pour votre titre H1 pour l’aperçu. 

**Remarque**: l’Informations doit avoir qu’un seul H1 en haut, sinon ils seront en rupture de production. Les H2 ne s’affichent pas. Utilisez donc des conventions en gras ou d’autres pour signer des sections distinctes. 
1. Ensuite, remplissez le corps de texte à l’aide du document de brouillon dans la section Insights client de la page Règle d’alchemy
    1. Les listes à puces sont corrects
    1. Listes numéroées également
    1. **Gras** et *italique* sont a-ok
    1. Les liens doivent toujours être des « liens vers le web » **/externes** **ou** des liens profonds vers des éléments d’interface utilisateur, et non des liens internes.
    1. Les images ne sont pas officiellement prises en charge pour le moment, mais elles sont dans la feuille de route.

Et c’est déjà un peu trop long. La meilleure pratique est d’environ 400 caractères ---------------------------------

Une fois votre contenu prêt, tirez-le vers la branche en direct. Ensuite, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. 