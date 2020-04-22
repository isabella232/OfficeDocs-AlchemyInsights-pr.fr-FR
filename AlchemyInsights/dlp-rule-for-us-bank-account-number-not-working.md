---
title: La règle DLP pour le numéro de compte bancaire américain ne fonctionne pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704037"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problèmes liés à DLP avec les numéros de compte bancaire américain

**Important**: En ces temps sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint en ligne et OneDrive demeurent très disponibles – Veuillez consulter [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes liés à DLP avec les numéros de compte bancaire américain**

Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de compte bancaire américain** lors de l’utilisation d’un type d’informations sensibles DLP dans O365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lors de l’évaluation.
  
Par exemple, pour une stratégie de **numéro de compte bancaire américain** configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche :
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 chiffres

- **[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 chiffres consécutifs.

- **[Checksum :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Une stratégie DLP est sûre à 75% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - L’expression régulière Regex_usa_bank_account_number trouve le contenu qui correspond au modèle

  - Un mot clé figurant dans la liste Keyword_usa_Bank_Account est trouvé.

    Par exemple, l’exemple suivant se déclenche pour la stratégie de **numéro de compte bancaire américain** : compte courant 78344011

Pour plus d’informations sur les éléments requis pour la détection d’un **numéro de compte bancaire américain** pour votre contenu, reportez-vous à la section suivante de cet article : [ce que recherche les types d’informations sensibles pour le numéro de compte bancaire américain](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  