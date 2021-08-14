---
title: Règle DLP pour le numéro de carte de crédit qui ne fonctionne pas
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005088"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problèmes DLP avec les numéros de carte de crédit

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes DLP avec les numéros de carte de crédit**

Avez-vous des problèmes avec la protection contre la  perte de données **(DLP)** qui ne fonctionne pas pour le contenu contenant un numéro de carte de crédit lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour déclencher la stratégie DLP lors de son évaluation. Par exemple,  pour une stratégie de carte de crédit configurée avec un niveau de confiance de 85 %, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche :
  
- **[Format :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 chiffres qui peuvent être mis en forme ou sans mise en forme (dddddd) et qui doivent réussir le test luhn.

- **[Modèle :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Modèle très complexe et robuste qui détecte les cartes de toutes les principales marques dans le monde, y compris Visa, MasterCard, Discover Card, JCB, American Express, les cartes-anniversaire et les cartes-mémoire.

- **[Checksum :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Oui, la checksum Luhn

- **[Définition :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Une stratégie DLP est 85 % de confiance qu’elle a détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - La fonction Func_credit_card trouve un contenu qui correspond au modèle.

  - L’une des affirmations suivantes est vraie :

  - Un mot clé figurant dans la liste Keyword_cc_verification est trouvé.

  - Un mot clé de Keyword_cc_name trouvé

  - La fonction Func_expiration_date trouve une date au format correct.

  - La passe de contrôle

    Par exemple, l’exemple suivant déclencherait une stratégie de numéro de carte de crédit DLP :

  - Visa : 4485 3647 3952 7352
  
  - Expire : 2/2009

Pour plus d’informations sur  les informations requises pour détecter un numéro de carte de crédit pour votre contenu, voir la section suivante de cet article : Ce que les types d’informations sensibles recherchent pour la carte [de crédit#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
À l’aide d’un autre type d’informations sensibles intégré, consultez l’article suivant pour plus d’informations sur ce qui est requis pour d’autres types : ce que les [types d’informations sensibles recherchent](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  