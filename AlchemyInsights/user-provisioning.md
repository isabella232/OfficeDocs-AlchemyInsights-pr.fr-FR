---
title: Provisionnement des utilisateurs
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
- "9004348"
- "8428"
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971337"
---
# <a name="user-provisioning"></a>Provisionnement des utilisateurs

- Utilisez la [fonctionnalité d’approvisionnement](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) à la demande pour mettre en service un utilisateur et obtenir des diagnostics détaillés sur les étapes à suivre.
- Pour résoudre les problèmes que vous rencontrez lors de l’approvisionnement d’utilisateurs et de groupes, consultez le guide de résolution des problèmes[Aucun utilisateur n'est approvisionné](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Si vous constatez que les utilisateurs ne sont pas approvisionnés, consultez [Journaux d’approvisionnement (aperçu)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) dans Azure Active Directory (AD). Recherchez les entrées de journal relatives à un utilisateur spécifique.
- Redémarrez régulièrement l’approvisionnement pour capturer les utilisateurs qui ont été manqués au cours d’un cycle d’approvisionnement précédent.
- L’utilisateur/groupe n’a peut-être pas été mis en service, car notre service n’a pas encore pu évaluer l’utilisateur. Examinez les instructions pour la durée de l’approvisionnement, ainsi que la barre de progression sur la page de configuration de l’approvisionnement. Si l’état stable spécifié dans la section détails supplémentaires se trouve avant la date de création/mise à jour/suppression de l’utilisateur, cela signifie que nous n’avons pas encore évalué l’utilisateur. Dans ce scénario, la meilleure chose à faire est d’attendre la fin du service d’approvisionnement. Si l’état stable est atteint, nous vous recommandons d’effectuer un redémarrage à partir de l’interface utilisateur dans le portail Azure.
  - Notez que notre service ne connaît que les modifications apportées à un utilisateur/groupe dans le système source (Azure Active Directory). Si un utilisateur/groupe est supprimé directement dans l’application (par exemple, ServiceNow), nous ne sommes pas conscients de ces modifications et ne les revenir pas en fonction de l’état de l’utilisateur dans le système source. Dans ce scénario, il est préférable de revenir à la modification directement dans l’application cible.
- Notre service a évalué l’utilisateur/le groupe et déterminé qu’il ne doit pas être provisioné :
  - Si vous avez affecté l’étendue à des utilisateurs et des groupes, vérifiez si l’utilisateur/groupe est affecté à l’application.
  - Si l’utilisateur/le groupe est affecté à l’application, assurez-vous qu’il n’est pas affecté au rôle d’accès par défaut. Ce rôle ne peut pas être utilisé pour l’approvisionnement.
  - Si vous avez définis un filtre d’attribution de l’ensemble des attributs, assurez-vous que l’utilisateur répond aux critères que vous avez spécifiés.
  - Si des utilisateurs existent déjà dans le système cible et l’état de l’utilisateur dans la correspondance source et cible, nous n’allons pas prendre d’autres mesures.
- Notre service a tenté de mettre en service l’utilisateur et il a échoué. Pour ces scénarios, examinez l’onglet Résolution des problèmes et recommandations des journaux d’approvisionnement :
  - Un attribut requis sur l’utilisateur peut être manquant dans Azure Active Directory ou ne correspond pas au format requis par l’application tierce. Par exemple, l’attribut Country d’un utilisateur peut être attribué aux États-Unis alors qu’il doit être US.
  - L’attribut est un attribut référent qui n’existe pas encore dans l’application cible. Un attribut référent est un attribut qui pointe vers un autre objet, par exemple, un utilisateur membre d’un groupe. L’ID de l’utilisateur se trouve dans l’attribut membre du groupe, mais ne peut être traitée que si l’objet utilisateur qu’il pointe existe déjà.
