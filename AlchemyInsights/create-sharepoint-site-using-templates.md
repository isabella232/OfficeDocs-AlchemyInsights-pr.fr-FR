---
title: Créer un site dans SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732219"
---
# <a name="create-sharepoint-sites-using-templates"></a>Créer des sites SharePoint à l’aide de modèles

La possibilité d’enregistrer un site en tant que modèle n’est pas prise en charge avec les sites d’équipe ou de communication modernes. Pour plus d’informations sur l’utilisation des modèles, consultez la rubrique [enregistrer, télécharger et télécharger un site SharePoint en tant que modèle](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Voici quelques problèmes/solutions courants relatifs à l’enregistrement d’un site ou d’une liste en tant que modèle dans SharePoint Online. 

**Le bouton enregistrer le modèle de site/liste n’est pas disponible ou est manquant**

Les administrateurs devront autoriser le script personnalisé à activer les fonctionnalités du modèle. Pour obtenir la procédure détaillée, des exemples et des considérations, voir 

- [Activer ou désactiver les scripts personnalisés](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication de SharePoint Server.

**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**

Il se peut que le modèle manque une [fonctionnalité](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) et ne s’active pas. Si la fonctionnalité n’est pas disponible pour l’activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.

- Vérifiez si des listes ou des bibliothèques dépassent le [seuil de limite d’affichage de liste](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments car cela peut bloquer la création d’un modèle de site.

- Le site utilise peut-être trop de ressources et, par conséquent, le modèle de site dépasse la limite de 50 Mo.


- Il existe des problèmes lors de l’affichage des données d’une liste qui utilise une colonne de recherche. Pour plus d’informations, reportez-vous à [la rubrique liste générée par un modèle n’affiche pas les données de la liste de recherche correcte dans SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Pour plus d’informations sur les problèmes et solutions courants, veuillez vérifier la [création et l’utilisation de modèles de sites](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



