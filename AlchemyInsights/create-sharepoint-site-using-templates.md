---
title: Créer un site dans SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755306"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c75f9-102">Créer des sites SharePoint à l’aide de modèles</span><span class="sxs-lookup"><span data-stu-id="c75f9-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c75f9-103">Les modèles de site SharePoint sont des définitions prédéfinies conçues autour d'un besoin d'entreprise particulier.</span><span class="sxs-lookup"><span data-stu-id="c75f9-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="c75f9-104">Pour plus d’informations, consultez la rubrique [utilisation de modèles pour créer différents types de sites SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="c75f9-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="c75f9-105">Voici quelques problèmes/solutions courants relatifs à l’enregistrement d’un site ou d’une liste en tant que modèle dans SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c75f9-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c75f9-106">**Le bouton enregistrer le modèle de site/liste n’est pas disponible ou est manquant**</span><span class="sxs-lookup"><span data-stu-id="c75f9-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c75f9-107">Les administrateurs devront autoriser le script personnalisé à activer les fonctionnalités du modèle.</span><span class="sxs-lookup"><span data-stu-id="c75f9-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c75f9-108">Pour obtenir la procédure détaillée, des exemples et des considérations, voir</span><span class="sxs-lookup"><span data-stu-id="c75f9-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c75f9-109">Activer ou désactiver les scripts personnalisés</span><span class="sxs-lookup"><span data-stu-id="c75f9-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c75f9-110">La commande Enregistrer le site en tant que modèle n’est pas prise en charge et peut entraîner des problèmes sur les sites qui utilisent l’infrastructure de publication de SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="c75f9-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c75f9-111">**Le modèle de site ne peut pas être créé ou ne fonctionne pas correctement**</span><span class="sxs-lookup"><span data-stu-id="c75f9-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c75f9-112">Il se peut que le modèle manque une [fonctionnalité](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) et ne s’active pas.</span><span class="sxs-lookup"><span data-stu-id="c75f9-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c75f9-113">Si la fonctionnalité n’est pas disponible pour l’activation dans la collection de sites actuelle, vous ne pouvez pas utiliser le modèle de site pour créer un site.</span><span class="sxs-lookup"><span data-stu-id="c75f9-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c75f9-114">Vérifiez si des listes ou des bibliothèques dépassent le [seuil de limite d’affichage de liste](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) de 5000 éléments car cela peut bloquer la création d’un modèle de site.</span><span class="sxs-lookup"><span data-stu-id="c75f9-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c75f9-115">Le site utilise peut-être trop de ressources et, par conséquent, le modèle de site dépasse la limite de 50 Mo.</span><span class="sxs-lookup"><span data-stu-id="c75f9-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c75f9-116">Il existe des problèmes lors de l’affichage des données d’une liste qui utilise une colonne de recherche.</span><span class="sxs-lookup"><span data-stu-id="c75f9-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c75f9-117">Pour plus d’informations, reportez-vous à [la rubrique liste générée par un modèle n’affiche pas les données de la liste de recherche correcte dans SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="c75f9-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="c75f9-118">Pour plus d’informations sur les problèmes et solutions courants, veuillez vérifier la [création et l’utilisation de modèles de sites](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="c75f9-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



