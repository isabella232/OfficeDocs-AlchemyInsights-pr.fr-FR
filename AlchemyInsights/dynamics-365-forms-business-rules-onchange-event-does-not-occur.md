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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529017"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange, événement ne se produit pas si le champ est modifié par programme

L’événement *OnChange* ne se produit pas si le champ est modifié par programmation à l’aide de l' *attribut.* méthode [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Si vous souhaitez que les gestionnaires d’événements de l’événement *OnChange* s’exécutent une fois que vous avez défini la valeur, vous devez utiliser l' *attribut formContext. Data. Entity.* méthode [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) dans votre code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
