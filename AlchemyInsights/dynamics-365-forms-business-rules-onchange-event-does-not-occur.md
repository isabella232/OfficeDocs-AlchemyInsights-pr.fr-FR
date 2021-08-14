---
title: Dynamics 365 Forms Business Rules - Business Rule Not Firing for a Form
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
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947297"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>L’événement OnChange ne se produit pas si le champ est modifié par programme

*L’événement OnChange* ne se produit pas si le champ est modifié par programme à l’aide de l’attribut.  [méthode setValue.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Si vous souhaitez que les handlers d’événements pour l’événement *OnChange* s’exécutent après avoir définie la valeur, vous devez utiliser la méthode [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) d’attribut *formContext.data.entity* dans votre code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
