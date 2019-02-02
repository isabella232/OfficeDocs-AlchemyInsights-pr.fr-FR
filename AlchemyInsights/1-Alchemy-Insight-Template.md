---
title: 'identique au nom de fichier est préférable [règle #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697128"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Requis Alchemy en-tête H1, H2 ne fonctionnent pas.
Meilleures pratiques et recommandations pour la création de Alchemy :

1. **Ne pas imbriquer Alchemy Insights dans les dossiers**- cela interrompt la structure d’url. Nous cherchons à corriger ce.
1. Fichiers dans le dossier **AlchemyInsights** doivent avoir des ID de la règle et le nom de la règle à partir du [portail partenaires Alchemy](https://alchemyportal.azurewebsites.net) dans le nom de fichier.
    1. exemple : ***976-How-to-enable-litigation-hold***
1. Utiliser les métadonnées en haut de ce fichier en tant que votre modèle. Rien d’autre n’est nécessaire.
1. Dans le [portail partenaires Alchemy](https://alchemyportal.azurewebsites.net), naviguez jusqu'à la section **client Insight titre :** et l’utilisation qui en tant que le démarrage d’un point du titre H1 l’aperçu. 
    > [!NOTE]
    > Alchemy Insights doit n'avoir qu’un seul H1 en haut ou erreurs en production. Utilisation de ce **gras** ou autres conventions pour indiquer des sections distinctes ne rendu de H2s.
1. Ensuite, renseignez le corps du texte à l’aide de la matière brouillon dans la section Détails du client de la page Alchemy règle
    1. Les listes à puces sont correctement
    1. Trop de listes numérotées
    1. **Gras** et *italique* sont a-ok
    1. Liens doivent toujours être **« des liens Web » / externe** OR **profond-des liens vers des éléments d’interface utilisateur**, les liens pas internes.

Et c’est vraiment déjà un peu trop long. Meilleure pratique consiste à environ 400 caractères---

Une fois votre contenu est prêt, l’extraction vers la branche live. Ensuite, accédez au [portail Alchemy](https://alchemyportal.azurewebsites.net) et entrez le nom de fichier dans le champ url. Assurez-vous que Insight révisé et publié indique « Oui », puis cliquez sur règle de mise à jour. **(Cette recherche plus attrayants dans la nouvelle version du portail - libération bientôt.)** 
 ![champ url](media/for-content-team.PNG)

