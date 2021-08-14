---
title: Règle DLP pour le numéro de compte bancaire américain ne fonctionne pas
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005016"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problèmes de DLP avec des numéros de compte bancaire aux États-Unis

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes de DLP avec des numéros de compte bancaire aux États-Unis**

Avez-vous des problèmes avec la protection contre la  perte de données **(DLP)** qui ne fonctionne pas pour le contenu contenant un numéro de compte bancaire américain lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lorsqu’elle est évaluée.
  
Par exemple,  pour une stratégie de numéro de compte bancaire aux États-Unis configurée avec un niveau de confiance de 85 %, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche :
  
- **[Format :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8 à 17 chiffres

- **[Modèle :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8 à 17 chiffres consécutifs.

- **[Checksum :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Une stratégie DLP est 75 % de confiance qu’elle a détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - L’expression régulière Regex_usa_bank_account_number trouve un contenu qui correspond au modèle

  - Un mot clé figurant dans la liste Keyword_usa_Bank_Account est trouvé.

    Par exemple, l’exemple suivant  déclencherait la stratégie de numéro de compte bancaire des États-Unis : compte 78344011

Pour plus d’informations sur  les informations requises pour détecter un numéro de compte bancaire américain pour votre contenu, voir la section suivante de cet article : Ce que les [types](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) d’informations sensibles recherchent pour le numéro de compte bancaire américain
  
À l’aide d’un autre type d’informations sensibles intégré, consultez l’article suivant pour plus d’informations sur ce qui est requis pour d’autres types : ce que les [types d’informations sensibles recherchent](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  