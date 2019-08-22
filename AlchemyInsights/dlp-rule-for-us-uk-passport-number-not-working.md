---
title: La règle DLP pour le numéro de passeport US/UK ne fonctionne pas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529917"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problèmes liés aux numéros de passeport DLP-US/UK

Avez-vous des problèmes avec la **protection contre la perte de données (DLP)** qui ne fonctionnent pas pour le contenu contenant un **numéro de passeport US/UK** lorsque vous utilisez un type d’informations sensibles DLP dans O365? Si c’est le cas, assurez-vous que votre contenu contient les informations nécessaires pour ce que la stratégie DLP recherche lors de l’évaluation.
  
Par exemple, pour une stratégie de **numéro de passeport US/UK** configurée avec un niveau de confiance de 75%, les éléments suivants sont évalués et doivent être détectés pour que la règle se déclenche
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Neuf chiffres

- **[Modèle:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Neuf chiffres consécutifs

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Non, il n’y a pas de checksum

- **[Définition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Une stratégie DLP est sûre à 75% d’avoir détecté ce type d’informations sensibles si, dans une proximité de 300 caractères:

  - La fonction Func_usa_uk_passport trouve un contenu qui correspond au modèle.

  - Un mot clé figurant dans la liste Keyword_passport est trouvé.

    Par exemple, l’exemple suivant se déclenche pour la stratégie de **numéro de passeport US/UK** : numéro de passeport américain 123456789

Pour plus d’informations sur les éléments requis pour la détection d’un numéro de passeport US/UK pour votre contenu, consultez la section suivante de cet article: [ce que les types d’informations sensibles recherchent sur le numéro de passeport US/UK](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
À l’aide d’un type d’informations sensibles intégré différent, consultez l’article suivant pour obtenir des informations sur les éléments requis pour les autres types: [ce que recherche les types d’informations sensibles](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  