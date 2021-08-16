---
title: Règle DLP pour le numéro de passeport États-Unis/Royaume-Uni ne fonctionne pas
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004944"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problèmes liés à la DLP : numéros de passeport des États-Unis/du Royaume-Uni

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes de DLP avec les numéros de passeport des États-Unis/du Royaume-Uni**

Avez-vous des problèmes avec la protection contre la perte de données **(DLP)** qui ne fonctionne pas pour le contenu contenant un numéro de passeport **américain/britannique** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lorsqu’elle est évaluée.
  
Par exemple, pour une stratégie de numéro de passeport **américaine/britannique** configurée avec un niveau de confiance de 75 %, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche.
  
- **[Format :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Neuf chiffres

- **[Modèle :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Neuf chiffres consécutifs

- **[Checksum :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Une stratégie DLP est 75 % de confiance qu’elle a détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.

  - Un mot clé figurant dans la liste Keyword_passport est trouvé.

    Par exemple, l’exemple suivant déclencherait la stratégie de numéro de passeport des **États-Unis/du** Royaume-Uni : numéro de passeport américain 123456789

Pour plus d’informations sur les informations requises pour la détection d’un numéro de passeport États-Unis/Royaume-Uni pour votre contenu, voir la section suivante de cet article : Ce que les types d’informations sensibles recherchent pour le numéro de passeport [États-Unis/Royaume-Uni](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
À l’aide d’un autre type d’informations sensibles intégré, consultez l’article suivant pour plus d’informations sur ce qui est requis pour d’autres types : ce que les [types d’informations sensibles recherchent](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  