---
title: Règle DLP pour le non-fonctionnement du SSN
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004980"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Problèmes DLP avec les numéros de sécurité sociale

**Important** : dans cette situation sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint Online et OneDrive demeurent très disponibles – Veuillez consulter [Ajustements temporaire des fonctionnalités SharePoint Online](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes DLP avec les SSN**

Avez-vous des problèmes avec la protection contre la perte de données **(DLP)** qui ne fonctionne pas pour le contenu contenant un numéro de sécurité sociale **(SSN)** lors de l’utilisation d’un type d’informations sensibles dans Microsoft 365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires à la recherche de la stratégie DLP. 
  
Par exemple, pour une stratégie SSN configurée avec un niveau de confiance de 85 %, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche :
  
- **[Format :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 chiffres, qui peuvent être dans un modèle formaté ou sans mise en forme

- **[Modèle :](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Quatre fonctions recherchent des SSN dans quatre modèles différents :

  - Func_ssn recherche des numéros de sécurité sociale avec une mise en forme fixe d’avant l’année 2011, mis en forme avec des tirets ou des espaces (ddd-dd-dddd OU ddd dd dddd)

  - Func_unformatted_ssn recherche des numéros de sécurité sociale avec une mise en forme fixe d’avant l’année 2011, avec neuf chiffres consécutifs non mis en forme (ddddddddd)

  - Func_randomized_formatted_ssn recherche des numéros de sécurité sociale d’après l’année 2011, mis en forme avec des tirets ou des espaces  (ddd-dd-dddd OU ddd dd dddd)

  - Func_randomized_unformatted_ssn recherche des numéros de sécurité sociale d’après l’année 2011, avec neuf chiffres consécutifs non mis en forme (ddddddddd)

- **[Checksum :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Une stratégie DLP est 85 % de confiance qu’elle a détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - La [fonction Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) trouve un contenu qui correspond au modèle.

  - Un mot clé figurant dans la liste [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) est trouvé. Exemples de mots clés :  *Sécurité sociale, Sécurité sociale#, Soc Sec ,SSN*  . Par exemple, l’exemple suivant déclencherait la stratégie SSN DLP : **SSN : 489-36-8350**
  
Pour plus d’informations sur les informations requises pour détecter les SSN pour votre contenu, voir la section suivante de cet article : Ce que les types d’informations sensibles recherchent pour les [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
À l’aide d’un autre type d’informations sensibles intégré, consultez l’article suivant pour plus d’informations sur ce qui est requis pour d’autres types : ce que les [types d’informations sensibles recherchent](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  