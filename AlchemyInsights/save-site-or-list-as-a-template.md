---
title: Enregistrer un site ou une liste en tant que modèle
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 73a32536995a604c734393c2300b4c9bb507e2b2
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770526"
---
# <a name="save-site-or-list-as-a-template"></a>Enregistrer un site ou une liste en tant que modèle

Les modèles de site SharePoint sont des définitions prédéfinies conçues autour d'un besoin d'entreprise particulier. Pour plus d’informations, consultez la rubrique [utilisation de modèles pour créer différents types de sites SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Voici quelques problèmes/solutions courants relatifs à l’enregistrement d’un site ou d’une liste en tant que modèle dans SharePoint Online.

Le **bouton enregistrer le modèle de site/liste n’est pas disponible ou est manquant**. 

- Les administrateurs devront autoriser le script personnalisé à activer les fonctionnalités du modèle. Pour obtenir la procédure détaillée, des exemples et des considérations, voir [autoriser ou empêcher les scripts personnalisés](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication de SharePoint Server.


**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**

- Il se peut que le modèle manque une [fonctionnalité](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) et ne s’active pas. Si la fonctionnalité n’est pas disponible pour l’activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.


- Vérifiez si des listes ou des bibliothèques dépassent le [seuil de limite d’affichage de liste](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments car cela peut bloquer la création d’un modèle de site.


- Le site utilise peut-être trop de ressources et par conséquent le modèle de site dépasse la limite de 50 mégaoctets (Mo).


- Il existe des problèmes lors de l’affichage des données d’une liste qui utilise une colonne de recherche. Pour plus d’informations, reportez-vous à [la rubrique liste générée par un modèle n’affiche pas les données de la liste de recherche correcte dans SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Pour plus d’informations sur les problèmes et solutions courants, reportez-vous à la référence, la [création et l’utilisation de modèles de sites](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

