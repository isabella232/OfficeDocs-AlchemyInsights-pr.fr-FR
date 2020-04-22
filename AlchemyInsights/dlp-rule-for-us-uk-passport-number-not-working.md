---
title: La règle DLP pour le numéro de passeport US/UK ne fonctionne pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714984"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problèmes liés aux numéros de passeport DLP-US/UK

**Important**: En ces temps sans précédent, nous prenons des mesures pour nous assurer que les services SharePoint en ligne et OneDrive demeurent très disponibles – Veuillez consulter [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) pour obtenir de plus amples renseignements.

**Problèmes liés à DLP avec les numéros de passeport US/UK**

Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de passeport US/UK** lorsque vous utilisez un type d’informations sensibles DLP dans O365 ? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lors de l’évaluation.
  
Par exemple, pour une stratégie de **numéro de passeport US/UK** configurée avec un niveau de confiance de 75%, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche
  
- **[Format :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neuf chiffres

- **[Modèle :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neuf chiffres consécutifs

- **[Checksum :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’y a pas de checksum

- **[Définition :](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Une stratégie DLP est sûre à 75% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères :

  - La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.

  - Un mot clé figurant dans la liste Keyword_passport est trouvé.

    Par exemple, l’exemple suivant se déclenche pour la stratégie de **numéro de passeport US/UK** : numéro de passeport américain 123456789

Pour plus d’informations sur les éléments requis pour la détection d’un numéro de passeport US/UK pour votre contenu, consultez la section suivante de cet article : [ce que les types d’informations sensibles recherchent sur le numéro de passeport US/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types : [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  