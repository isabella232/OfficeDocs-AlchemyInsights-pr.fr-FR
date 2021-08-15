---
title: Problème avec un seul utilisateur
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960149"
---
# <a name="problem-with-single-user"></a>Problème avec un seul utilisateur

- L’utilisateur n’a peut-être pas été mis en service, car le service n’a pas encore eu l’occasion d’évaluer l’utilisateur. Examinez les instructions pour la durée de l’approvisionnement, ainsi que la barre de progression sur la page de configuration de l’approvisionnement. Si l’état stable spécifié dans la section détails supplémentaires se trouve avant la date de création/mise à jour/suppression de l’utilisateur, cela signifie que nous n’avons pas encore évalué l’utilisateur. Dans ce scénario, la meilleure chose à faire est d’attendre la fin du service d’approvisionnement.

  - Notez que notre service ne connaît que les modifications apportées à un utilisateur dans le système source (Cloud HR). Il doit y avoir une modification valide dans le système source pour Azure AD afin de détecter la modification et de la faire circuler dans Active Directory.
- Le service d’approvisionnement a évalué l’utilisateur et déterminé qu’il ne doit pas être provisioné :
  - Si vous avez définis un filtre d’attribution de l’ensemble des attributs, assurez-vous que l’utilisateur répond aux critères que vous avez spécifiés.
  - Si des utilisateurs existent déjà dans le système cible et l’état de l’utilisateur dans la correspondance source et cible, nous n’allons pas prendre d’autres mesures.
- Le service d’approvisionnement a tenté de mettre en service l’utilisateur et a échoué. Pour ces scénarios, examinez l’onglet Résolution des problèmes et recommandations des journaux d’approvisionnement :
  - Un attribut requis sur l’utilisateur peut être manquant dans Active Directory local ou Azure AD. Par exemple, les règles de génération userPrincipalName ou sAMAccountName ne génèrent pas la bonne valeur.
  - L’attribut correspondant (généralement employeeId) ne se réssolvant pas en un utilisateur unique dans Active Directory local ou Azure AD. Par exemple, deux utilisateurs ont le même employeeId dans AD et le service renvoie un code d’erreur qui indique des entrées cibles en double pour la même entrée source.

Pour consulter les journaux d’un utilisateur et d’un groupe, consultez les journaux d’approvisionnement pour un [problème avec un utilisateur spécifique.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
