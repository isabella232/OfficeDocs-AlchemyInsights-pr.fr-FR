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
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712182"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP peut avoir besoin d’un type personnalisé

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**DLP peut nécessiter un type d’informations personnalisé**

Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles de votre organisation. Dans certains cas, vous devrez peut-être créer votre propre type d’informations sensibles **personnalisées** pour protéger les données de votre organisation.

Par exemple, votre organisation peut avoir besoin d’identifier et de protéger des ID d’employés ou d’autres données dans un format spécifique à votre organisation. Si c’est le cas, consultez les articles suivants pour plus d’informations.
  
 **Personnaliser un type d’informations sensibles intégré**
  
Si un type d’informations sensibles intégré répond à vos besoins avec seulement quelques ajustements, vous pouvez [personnaliser un type d’informations sensibles intégré](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves de prise en charge telles qu’une date ou une adresse.
  
 **Créer un type d’informations sensibles personnalisé**
  
Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez [créer un type d’informations sensibles personnalisé](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) dans l’interface utilisateur du centre de sécurité & conformité.
  
**Créer un type d’informations sensibles personnalisé dans l’interface PowerShell du Centre de sécurité et conformité**

Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez [créer un type d’informations sensibles personnalisé dans la sécurité & Centre de conformité PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles.
