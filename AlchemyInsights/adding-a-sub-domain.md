---
title: Ajout d’un sous-domaine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475952"
---
# <a name="adding-a-sub-domain"></a>Ajout d’un sous-domaine

Les sous-domaines peuvent être ajoutés au même client ou à un autre client que le domaine parent. Dans les deux cas, vous devez gérer vos propres paramètres DNS sur le site web de votre bureau d’enregistrement. Si vous avez laissé Microsoft gérer vos paramètres DNS avec des enregistrements NS, ou si vous avez acheté le domaine auprès de Microsoft, vous ne pouvez pas ajouter de sous-domaines sans modifier ce paramètre au départ.

Ajoutez d’abord le domaine parent, puis le sous-domaine. Si le sous-domaine se trouve dans le même client, aucune vérification supplémentaire n’est nécessaire. Si vous ajoutez le sous-domaine à un client distinct, l’enregistrement txt DNS est requis pour la vérification de la propriété avant d’ajouter le domaine et les enregistrements DNS supplémentaires pour les services sélectionnés.

- Pour ajouter un domaine ou un sous-domaine, suivez l’Assistant Ajouter un [domaine,](https://admin.microsoft.com/Adminportal#/Domains/Wizard)ou ajoutez manuellement le domaine ou le sous-domaine en allant dans Définir les domaines   >  **Ajouter**  >  **un domaine.**

Si nécessaire :

- Pour modifier les personnes qui gèrent vos paramètres DNS pour un domaine existant, sélectionnez **Paramètres** Domaines, cochez la case en regard du domaine, puis sélectionnez Gérer  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **DNS.** Dans l’Assistant, sélectionnez Ajouter vos propres enregistrements **DNS** et terminez l’Assistant.
- Pour ajouter des sous-domaines à un domaine acheté par Microsoft, transférez d’abord le domaine vers un autre bureau d’enregistrement, puis a effectuer les changements ci-dessus pour gérer vos propres enregistrements DNS. Pour obtenir des instructions, [voir Transférer un domaine de Microsoft vers un autre hôte.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Si vous recevez une erreur selon qui votre domaine est déjà utilisé par d’autres membres ou personnes de votre organisation, vous devez d’abord prendre le contrôle de ce compte non utilisé avant d’utiliser le domaine. Pour obtenir des instructions, voir Prendre en compte un répertoire non gérant en tant [qu’administrateur dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
