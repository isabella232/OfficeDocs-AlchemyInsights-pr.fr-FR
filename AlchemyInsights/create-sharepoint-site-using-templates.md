---
title: Créer un site dans SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 2097933dd20f326a7bda2151596d514c37d566ff
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717765"
---
# <a name="create-sharepoint-sites-using-templates"></a>Créer des sites SharePoint à l’aide de modèles

Les modèles de site SharePoint sont des définitions prédéfinies conçues autour d'un besoin d'entreprise particulier. Pour plus d’informations, consultez la rubrique <a href="https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4">utilisation de modèles pour créer différents types de sites SharePoint.</a></span></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Voici quelques problèmes/solutions courants relatifs à l’enregistrement d’un site ou d’une liste en tant que modèle dans SharePoint Online.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Le bouton enregistrer le modèle de site/liste n’est pas disponible ou est manquant.</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Les administrateurs devront autoriser le script personnalisé à activer les fonctionnalités du modèle. Pour obtenir la procédure détaillée, des exemples et des considérations, voir </span> </span> <a style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">autoriser ou empêcher les scripts personnalisés</a>.</li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication de SharePoint Server.</span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement</span></u></strong></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Il se peut que le modèle <a href="https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx"></a> manque une fonctionnalité&rsquo;et qu’il ne soit pas activé. Si la fonctionnalité n’est pas disponible pour l’activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Vérifiez si des listes ou des bibliothèques dépassent le <a href="https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59">seuil de limite d’affichage de liste de</a> 5000 éléments car cela peut bloquer la création d’un modèle de site.</span></li> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Le site utilise peut-être trop de ressources et, par conséquent, le modèle de site dépasse la limite de 50 Mo.</span></li> <li>
Il existe des problèmes lors de l’affichage des données d’une liste qui utilise une colonne de recherche. Pour plus d’informations, </span> <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"> <a style="box-sizing: border-box; -webkit-text-stroke-width: 0px; word-spacing: 0px;" href="https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a"> <span style="color: #0067b8; text-decoration: none; text-underline: none;">reportez-vous à&rsquo;la rubrique liste générée par un modèle n’affiche pas les données de la liste de recherche correcte dans SharePoint Online.

Pour plus d’informations sur les problèmes et solutions courants, veuillez <a href="https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989">vérifier la création et l’utilisation de modèles de sites.



