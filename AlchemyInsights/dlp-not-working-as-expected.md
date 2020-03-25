---
title: DLP ne fonctionne pas comme prévu
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932620"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne fonctionne pas comme prévu

**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan. Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde. Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.

Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine. Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires. Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.

 **Configuration de DLP**

Rencontrez-vous des problèmes avec la **protection contre la perte de données (DLP)** dans Office 365 ne fonctionnent pas comme prévu ? Si c’est le cas, assurez-vous que votre **stratégie DLP** est correctement configurée et que vos données contiennent ce que la **stratégie DLP** recherche lors de l’évaluation.
  
Les stratégies DLP vous permettent d’identifier et de protéger les informations sensibles de votre organisation. Pour configurer les stratégies DLP, utilisez les informations [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Stratégies DLP**
  
Lors de l’utilisation des **types d’informations sensibles intégrés** dans le centre de sécurité et de conformité Office 365, les stratégies DLP recherchent des éléments et des modèles spécifiques lors de la détection de ces types sensibles.
  
- **Types d’informations sensibles intégrés**

    Pour plus d’informations sur les types sensibles intégrés et sur ce qu’une stratégie DLP doit rechercher lors de la détection du type sensible, voir : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Types d’informations sensibles personnalisés**

    Si vous essayez de créer des types d’informations sensibles personnalisés, utilisez l’article suivant pour obtenir des informations sur la création d’un type de données sensibles personnalisé : [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Tester une stratégie DLP**

Pour tester vos données à l’aide d’un type d’informations sensibles intégré ou personnalisé, utilisez l’option **type de test** sous types d’informations**sensibles**sur les **classifications** > . Pour plus d’informations, consultez la rubrique [test des types d’informations sensibles personnalisés](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Rapports**
  
- Obtenez des données sensibles à l’aide des [rapports DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Consultez les détails spécifiques de l’événement à l’aide d’un [rapport d’incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
