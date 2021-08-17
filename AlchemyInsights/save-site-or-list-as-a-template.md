---
title: Enregistrer un site ou une liste en tant que modèle
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109202"
---
# <a name="save-site-or-list-as-a-template"></a>Enregistrer un site ou une liste en tant que modèle

Les modèles de site SharePoint sont des définitions prédéfinies conçues autour d'un besoin d'entreprise particulier. Pour plus d’informations, voir [Utilisation de modèles pour créer différents types](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)SharePoint sites.

Voici quelques problèmes/solutions courants concernant l’enregistrement d’un site ou d’une liste en tant que modèle dans SharePoint Online.

**Le bouton Enregistrer le modèle de site/liste n’est pas disponible ou manquant.** 

- Les administrateurs devront autoriser les scripts personnalisés pour activer les fonctionnalités de modèle. Pour obtenir la procédure détaillée, des exemples et des considérations, voir [Autoriser ou empêcher les scripts personnalisés.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication SharePoint Server.


**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**

- Il est possible que le modèle ne dispose [pas d’une](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) fonctionnalité et qu’il ne s’active pas. Si la fonctionnalité n’est pas disponible pour activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.


- Vérifiez si les listes ou les bibliothèques dépassent le [seuil de l’affichage de liste](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments, car cela peut empêcher la création d’un modèle de site.


- Le site utilise peut-être trop de ressources et, par conséquent, le modèle de site dépasse la limite de 50 mégaoctets (Mo).


- Il existe des problèmes lors de l’affichage de données à partir d’une liste qui utilise une colonne de recherche. Pour plus d’informations, voir La liste générée par un [modèle n’affiche](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)pas les données de la liste de recherche correcte dans SharePoint Online.


Pour plus d’informations sur les problèmes courants et les solutions, veuillez référencer, [créer et utiliser des modèles de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

