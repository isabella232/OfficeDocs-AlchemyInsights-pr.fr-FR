---
title: Enregistrer un site ou une liste en tant que modèle
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243327"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="37f1a-102">Enregistrer un site ou une liste en tant que modèle</span><span class="sxs-lookup"><span data-stu-id="37f1a-102">Save site or list as a template</span></span>

<span data-ttu-id="37f1a-103">Les modèles de site SharePoint sont des définitions prédéfinies conçues autour d'un besoin d'entreprise particulier.</span><span class="sxs-lookup"><span data-stu-id="37f1a-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="37f1a-104">Pour plus d'informations, consultez la rubrique [utilisation de modèles pour créer différents types de sites SharePoint](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="37f1a-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="37f1a-105">Voici quelques problèmes/solutions courants relatifs à l'enregistrement d'un site ou d'une liste en tant que modèle dans SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="37f1a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="37f1a-106">Le **bouton enregistrer le modèle de site/liste n'est pas disponible ou est manquant**.</span><span class="sxs-lookup"><span data-stu-id="37f1a-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="37f1a-107">Les administrateurs devront autoriser le script personnalisé à activer les fonctionnalités du modèle.</span><span class="sxs-lookup"><span data-stu-id="37f1a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="37f1a-108">Pour obtenir la procédure détaillée, des exemples et des considérations, voir [autoriser ou empêcher les scripts personnalisés](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="37f1a-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="37f1a-109">La commande Enregistrer le site en tant que modèle n'est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l'infrastructure de publication de SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="37f1a-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="37f1a-110">**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**</span><span class="sxs-lookup"><span data-stu-id="37f1a-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="37f1a-111">Il se peut que le modèle manque une [fonctionnalité](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) et ne s'active pas.</span><span class="sxs-lookup"><span data-stu-id="37f1a-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="37f1a-112">Si la fonctionnalité n'est pas disponible pour l'activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.</span><span class="sxs-lookup"><span data-stu-id="37f1a-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="37f1a-113">Vérifiez si des listes ou des bibliothèques dépassent le [seuil de limite d'affichage de liste](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments car cela peut bloquer la création d'un modèle de site.</span><span class="sxs-lookup"><span data-stu-id="37f1a-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="37f1a-114">Le site utilise peut-être trop de ressources et par conséquent le modèle de site dépasse la limite de 50 mégaoctets (Mo).</span><span class="sxs-lookup"><span data-stu-id="37f1a-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="37f1a-115">Il existe des problèmes lors de l'affichage des données d'une liste qui utilise une colonne de recherche.</span><span class="sxs-lookup"><span data-stu-id="37f1a-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="37f1a-116">Pour plus d'informations, reportez-vous à [la rubrique liste générée par un modèle n'affiche pas les données de la liste de recherche correcte dans SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="37f1a-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="37f1a-117">Pour plus d'informations sur les problèmes et solutions courants, reportez-vous à la référence, la [création et l'utilisation de modèles de sites](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="37f1a-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

