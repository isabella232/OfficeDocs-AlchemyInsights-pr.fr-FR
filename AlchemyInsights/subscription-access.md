---
title: Accès aux abonnements
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48773773"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Impossible de se connecter à Azure en raison de problèmes de navigateur (blocage du navigateur, continuité de l’exécution, pas chargement, etc.)

Vous pouvez être concerné par une panne. Vérifiez s’il existe une panne en cours : état d' [intégrité Azure](https://status.azure.com/status/history/).

Déconnectez-vous de toutes les sessions Azure actives. Démarrez un mode Incognito ou de votre navigateur Web.

Vous pouvez également essayer d’actualiser le navigateur, d’utiliser un autre navigateur, de supprimer les cookies de cache si vous ne travaillez pas.

En savoir plus : [résoudre les problèmes de connexion](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Impossible d’accéder aux abonnements**

Dans le [portail Azure](https://portal.azure.com/), assurez-vous que le répertoire Azure approprié est sélectionné à partir du compte dans le coin supérieur droit.

Dans le [Centre de comptes Azure](https://account.windowsazure.com/Subscriptions), assurez-vous que le compte utilisé est l’administrateur de compte.

En savoir plus : [dépanner aucun abonnement trouvé](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Impossible d’accéder à l’historique de facturation**

L’administrateur de compte doit s’assurer que l’utilisateur qui accède aux informations de facturation est ajouté à Azure Active Directory en tant qu’utilisateur invité : [Ajouter ou supprimer un nouvel utilisateur](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

L’utilisateur doit ensuite disposer d’un rôle d’administrateur global : [attribuer un rôle aux utilisateurs](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Publier ce message, l’utilisateur peut bénéficier d’un accès de facturation à l’aide de stratégies RBAC : [accorder l’accès à la facturation](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documents recommandés**

-   [Je ne parviens pas à me connecter pour gérer mon abonnement Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)