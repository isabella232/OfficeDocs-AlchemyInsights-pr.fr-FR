---
title: Règles métier des formulaires Dynamics 365-la règle d’entreprise ne se déclenche pas pour un formulaire
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769337"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange, événement ne se produit pas si le champ est modifié par programme

L’événement *OnChange* ne se produit pas si le champ est modifié par programmation à l’aide de l' *attribut.* méthode [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Si vous souhaitez que les gestionnaires d’événements de l’événement *OnChange* s’exécutent une fois que vous avez défini la valeur, vous devez utiliser la méthode [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) de l' *attribut formContext. Data. Entity* dans votre code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
