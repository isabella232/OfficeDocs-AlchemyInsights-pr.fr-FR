---
title: La DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079700"
---
# <a name="dlp-not-working-as-expected"></a>La DLP ne fonctionne pas comme prévu

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

 **Configuration de la DLP**

Avez-vous des problèmes avec la protection contre la perte de données **(DLP)** Office 365 ne fonctionne pas comme prévu ? Si c’est le cas, assurez-vous que votre stratégie **DLP** est correctement définie et que vos données contiennent ce que la stratégie **DLP** recherche lorsqu’elle est évaluée.
  
Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles dans votre organisation. Pour configurer des stratégies DLP, utilisez les informations [ici.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Ce que les stratégies DLP recherchent**
  
Lorsque vous utilisez les **types** d’informations sensibles intégrés dans les centres de sécurité et conformité, les stratégies DLP recherchent des modèles et des éléments spécifiques lors de la détection de ces types sensibles.
  
- **Types d’informations sensibles intégrés**

    Pour plus d’informations sur les types sensibles intégrés et ce qu’une stratégie DLP recherche lors de la détection du type Sensible, voir : Ce que les types d’informations sensibles [recherchent.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Types d’informations sensibles personnalisés**

    Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour plus d’informations sur la création d’un type d’informations sensibles personnalisé : Créer un [type d’informations sensibles personnalisé.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Tester une stratégie DLP**

Pour tester vos données avec un type d’informations sensibles intégré ou personnalisé, utilisez l’option **Type** de test sous Classifications Types d’informations   >  **sensibles.** Pour plus d’informations, voir [Tester les types d’informations sensibles personnalisés.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Rapports**
  
- Obtenez des informations sur les données sensibles avec [les rapports DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Consultez les détails spécifiques de l’événement avec un [rapport d’incident.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)
