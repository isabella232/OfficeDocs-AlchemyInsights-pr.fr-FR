---
title: DLP peut avoir besoin d’un type personnalisé
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030792"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP peut avoir besoin d’un type personnalisé

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**La DLP peut nécessiter un type d’informations personnalisé**

Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles au sein de votre organisation. Dans certains scénarios, vous devrez peut-être créer votre **propre** type d’informations sensibles personnalisé pour protéger les données de votre organisation.

Par exemple, votre organisation peut avoir besoin d’identifier et de protéger les ID d’employé ou d’autres données dans un format spécifique à votre organisation. Si c’est le cas, consultez les articles suivants pour plus d’informations.
  
 **Personnaliser un type d’informations sensibles intégré**
  
Si un type d’informations sensibles intégré répond à vos besoins avec quelques ajustements, vous pouvez personnaliser un type d’informations sensibles [intégré.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves justificatives telles qu’une date ou une adresse.
  
 **Créer un type d’informations sensibles personnalisé**
  
Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez créer un [type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) d’informations sensibles personnalisé dans l’interface utilisateur du Centre de sécurité & conformité.
  
**Créer un type d’informations sensibles personnalisé dans l’interface PowerShell du Centre de sécurité et conformité**

Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez créer un type d’informations sensibles personnalisé dans le Centre de sécurité & conformité [PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles.
