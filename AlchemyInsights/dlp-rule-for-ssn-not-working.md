---
title: Règle DLP pour numss ne fonctionnant pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704083"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problèmes liés à DLP avec des numéros de sécurité sociale

**Important**: En ces temps sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint en ligne et OneDrive demeurent très disponibles – Veuillez consulter [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes liés à DLP avec numéros**

Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de sécurité sociale** lors de l’utilisation d’un type d’informations sensibles dans Office 365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP examine. 
  
Par exemple, pour une stratégie de numéro de sécurité sociale configurée avec un niveau de confiance de 85%, les éléments suivants sont évalués et doivent être détectés pour le déclenchement de la règle :
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 chiffres, qui peuvent être dans un modèle mis en forme ou non mis en forme

- **[Modèle :](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatre fonctions recherchent numéros dans quatre modèles différents :

  - Func_ssn recherche des numéros de sécurité sociale avec une mise en forme fixe d’avant l’année 2011, mis en forme avec des tirets ou des espaces (ddd-dd-dddd OU ddd dd dddd)

  - Func_unformatted_ssn recherche des numéros de sécurité sociale avec une mise en forme fixe d’avant l’année 2011, avec neuf chiffres consécutifs non mis en forme (ddddddddd)

  - Func_randomized_formatted_ssn recherche des numéros de sécurité sociale d’après l’année 2011, mis en forme avec des tirets ou des espaces  (ddd-dd-dddd OU ddd dd dddd)

  - Func_randomized_unformatted_ssn recherche des numéros de sécurité sociale d’après l’année 2011, avec neuf chiffres consécutifs non mis en forme (ddddddddd)

- **[Checksum :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Une stratégie DLP est sûre à 85% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - La [fonction Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) trouve le contenu qui correspond au modèle.

  - Un mot clé figurant dans la liste [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) est trouvé. Exemples de mots clés : *Social Security, Social Security #, SOC sec, SSN* . Par exemple, l’exemple suivant se déclenche pour la stratégie SSN DLP : **SSN : 489-36-8350**
  
Pour plus d’informations sur les éléments requis pour la détection de numéros pour votre contenu, consultez la section suivante de cet article : [ce que recherche les types d’informations sensibles pour numéros](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  