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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057964"
---
# <a name="create-sharepoint-sites-using-templates"></a>Créer des sites SharePoint à l’aide de modèles

La possibilité d’enregistrer un site en tant que modèle n’est pas prise en charge avec les sites d’équipe ou de communication modernes. Pour plus d’informations sur l’utilisation des modèles, voir [Enregistrer, télécharger et charger un site SharePoint en tant que modèle](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Voici quelques problèmes/solutions courants concernant l’enregistrement d’un site ou d’une liste en tant que modèle dans Sharepoint Online. 

**Le bouton Enregistrer le modèle de site/liste n’est pas disponible ou manquant**

Les administrateurs devront autoriser les scripts personnalisés pour activer les fonctionnalités de modèle. Pour obtenir la procédure détaillée, des exemples et des considérations, voir 

- [Autoriser ou empêcher les scripts personnalisés](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication SharePoint Server.

**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**

Il est possible que le modèle ne dispose [pas d’une](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) fonctionnalité et qu’il ne s’active pas. Si la fonctionnalité n’est pas disponible pour activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.

- Vérifiez si les listes ou les bibliothèques dépassent le [seuil de l’affichage de liste](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments, car cela peut empêcher la création d’un modèle de site.

- Il est possible que le site utilise trop de ressources. par conséquent, le modèle de site dépasse la limite de 50 Mo.


- Il existe des problèmes lors de l’affichage de données à partir d’une liste qui utilise une colonne de recherche. Pour plus d’informations, consultez [La liste générée par un modèle n’affiche pas les données de la liste de recherche correcte dans SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Pour plus d’informations sur les problèmes et solutions courants, consultez [Créer et utiliser des modèles de site.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



