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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446689"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP peut avoir besoin d’un type personnalisé

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**La DLP peut nécessiter un type d’informations personnalisé**

Avec une stratégie de protection contre la perte de données (DLP), vous pouvez identifier et protéger les données sensibles au sein de votre organisation. Dans certains scénarios, vous devrez peut-être créer votre propre type d’informations sensibles personnalisé pour protéger les données de votre organisation. Pour plus d’informations, voir [En savoir plus sur les types d’informations sensibles](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) et les définitions d’entité des types [d’informations sensibles.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Pour plus d’informations sur la création de stratégies et de types d’informations sensibles personnalisés, voir : 

**Personnaliser un type d’informations sensibles intégré**

Si un type d’informations sensibles intégré répond à vos besoins avec quelques ajustements, voir Personnaliser un [type d’informations sensibles intégré.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Par exemple, vous pouvez ajouter ou supprimer des mots clés, ou ajouter ou supprimer des preuves justificatives telles qu’une date ou une adresse.

**Créer un type d’informations sensibles personnalisé**

Toutefois, si vous devez identifier et protéger un autre type d’informations sensibles, vous pouvez créer un type d’informations sensibles personnalisé dans le Centre de conformité Microsoft 365. Pour plus d’informations, [consultez La mise en place des types d’informations sensibles personnalisés.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Créer un type d’informations sensibles personnalisé dans l’interface PowerShell du Centre de sécurité et conformité**

Enfin, si l’interface utilisateur ne fournit pas toutes les options dont vous avez besoin, vous pouvez créer un type d’informations sensibles personnalisé dans le Centre de sécurité & conformité PowerShell. En commençant par un fichier XML, vous pouvez utiliser toutes les options disponibles. Pour plus d’informations, voir [Créer un type d’informations sensibles personnalisé à l’aide de PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Pour tester d’abord votre stratégie en mode test, voir Implémenter la stratégie en [mode test](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) et créer, tester et régler une [stratégie DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 