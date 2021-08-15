---
title: Accès à l’abonnement
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999238"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Impossible de se connecter à Azure en raison de problèmes de navigateur (le navigateur se bloque, continue de tourner, ne se charge pas, etc.)

Vous pouvez être touché par une panne. Vérifiez s’il existe une panne en cours : [État d’état d’santé Azure.](https://status.azure.com/status/history/)

Veuillez vous déconnecter de toutes les sessions Azure actives. Démarrez un mode privé ou incognito de votre navigateur web.

Vous pouvez également essayer d’actualiser le navigateur, d’utiliser un autre navigateur et de supprimer les cookies de cache si la procédure ci-dessus ne fonctionne pas.

En savoir plus : [résoudre les problèmes de la signature](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Impossible d’accéder aux abonnements**

Dans le [portail Azure,](https://portal.azure.com/)assurez-vous que le répertoire Azure correct est sélectionné à partir du compte en haut à droite.

Dans le [Centre de comptes Azure,](https://account.windowsazure.com/Subscriptions)assurez-vous que le compte utilisé est l’administrateur du compte.

En savoir plus : [Résoudre les problèmes d’absence d’abonnements trouvés](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Impossible d’accéder à l’historique de facturation**

L’administrateur de compte doit s’assurer que l’utilisateur accédant aux informations de facturation est ajouté dans Azure Active Directory en tant qu’utilisateur invité : Ajoutez ou supprimez [un nouvel utilisateur.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

L’utilisateur doit ensuite se voir attribuer un rôle d’administrateur global : [attribuer un rôle aux utilisateurs.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documents Recommandés**

-   [Je ne peux pas me connecter pour gérer mon abonnement Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)