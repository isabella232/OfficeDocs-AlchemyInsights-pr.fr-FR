---
title: Règles métier des formulaires Dynamics 365-la règle d’entreprise ne se déclenche pas pour un formulaire
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711489"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="6cb6a-102">OnChange, événement ne se produit pas si le champ est modifié par programme</span><span class="sxs-lookup"><span data-stu-id="6cb6a-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="6cb6a-103">L’événement *OnChange* ne se produit pas si le champ est modifié par programmation à l’aide de l' *attribut.* méthode [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="6cb6a-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="6cb6a-104">Si vous souhaitez que les gestionnaires d’événements de l’événement *OnChange* s’exécutent une fois que vous avez défini la valeur, vous devez utiliser la méthode [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) de l' *attribut formContext. Data. Entity* dans votre code.</span><span class="sxs-lookup"><span data-stu-id="6cb6a-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
