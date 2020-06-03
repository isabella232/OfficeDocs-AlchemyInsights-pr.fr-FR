---
title: DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507476"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne fonctionne pas comme prévu

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

 **Configuration de DLP**

Rencontrez-vous des problèmes avec la **protection contre la perte de données (DLP)** dans Office 365 ne fonctionnent pas comme prévu ? Si c’est le cas, assurez-vous que votre **stratégie DLP** est correctement configurée et que vos données contiennent ce que la **stratégie DLP** recherche lors de l’évaluation.
  
Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles de votre organisation. Pour configurer les stratégies DLP, utilisez les informations [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Stratégies DLP**
  
Lors de l’utilisation des **types d’informations sensibles intégrés** dans les centres de sécurité et de conformité, les stratégies DLP recherchent des éléments et des modèles spécifiques lors de la détection de ces types sensibles.
  
- **Types d’informations sensibles intégrés**

    Pour plus d’informations sur les types sensibles intégrés et sur ce qu’une stratégie DLP doit rechercher lors de la détection du type sensible, voir : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Types d’informations sensibles personnalisés**

    Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour obtenir des informations sur la création d’un type de données sensibles personnalisé : [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Tester une stratégie DLP**

Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations sensibles sur les **classifications**  >  **Sensitive info types**. Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapports**
  
- Obtenez des données sensibles à l’aide des [rapports DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Consultez les détails spécifiques de l’événement à l’aide d’un [rapport d’incident](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
