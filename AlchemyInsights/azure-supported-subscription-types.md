---
title: Types d’abonnements pris en charge
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791396"
---
# <a name="supported-subscription-types"></a>Types d’abonnements pris en charge

Veuillez consultez les types d’abonnements pris en charge pour continuer.

[Types d’abonnements pris en charge](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Transférer la propriété de facturation**

Portail Azure comme [Administrateur de Compte](https://ms.portal.azure.com/) du compte de facturation qui contient l’abonnement que vous voulez transférer

- Recherchez sur **Gestion des coûts + Facturation** . Sélectionnez **Abonnements** dans le volet gauche. Selon l’accès, vous devrez peut-être sélectionner une étendue de facturation, puis **Abonnements** ou **Abonnements Azure** .
- Sélectionnez l’option Transférer la propriété de facturation pour l’abonnement que vous voulez transférer
- Entrez l’adresse e-mail d’un utilisateur qui est un administrateur de facturation du compte qui sera le nouveau propriétaire de l’abonnement, puis sélectionnez **envoyer une demande de transfert**
- L’utilisateur reçoit un e-mail contenant des instructions pour examiner votre demande de transfert. Pour approuver la demande de transfert, l’utilisateur sélectionne le lien dans l’email et suit les instructions.

Remarque: Si vous transférez la propriété de facturation à, un compte d’utilisateur dans un autre client Azure AD , toutes les attributions du [contrôle d’accès basé sur le rôle (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) servant à gérer les ressources dans l’abonnement sont supprimées définitivement. Seul le nouveau propriétaire peut accéder à la gestion des ressources dans l’abonnement. Pour plus d’informations, consultez [transfert d’un abonnement à un utilisateur dans un autre client Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Transférer la Propriété de l’Abonnement**

Les conditions préalables du transfert de la propriété d’abonnement relatives à l’accès basé sur le rôle (RBAC) pour gérer les ressources dans l’abonnement perdent leur accès. Pour plus d’informations sur l’ajout d’un abonnement existant à un client, consultez [Associer ou ajouter un abonnement Azure à Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Le transfert d’abonnement avec un montant non payé existant du cycle de facturation actuel ne sera pas transféré vers le nouvel instrument de paiement dans le nouveau compte. La seule information disponible pour les utilisateurs dans le nouveau compte est le coût de l’abonnement du dernier mois. Le reste de l’historique des activités et de la facturation n’est pas transféré avec l’abonnement.
- Transférer la propriété de facturation des abonnements Accord Entreprise(EA) est actuellement pris en charge dans le portail Accord Entreprise uniquement
- Le transfert d’un abonnement orienté vers la solvabilité, tel que Visual Studio, BizSpark, Microsoft Partner Network vers un nouvel utilisateur, nécessite une licence réseau de partenaires Visual Studio/Microsoft pour accepter la demande de transfert.
- Toutes les ressources telles que les Machines Virtuelles, les disques et les sites Web sont transférées vers le nouveau compte. Les ressources suivantes peuvent être affectées dans un transfert d’abonnement inter-clients:

**Services de Domaine Azure AD**

Azure Key Vault

- [Les utilisateurs et bases de données liés à SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) peuvent être affectés, si le client utilise une authentification liée à Azure Active Directory
- La fonction **Services d’Application** configurée avec Azure Active Directory peut être affectée
- Les comptes Services **Visual Studio Team** connectés à des abonnements Azure peuvent perdre momentanément l’accès lorsque l’abonnement Azure connecté est annulé

**Documents recommandés**

Étapes suivant l’acceptation de la propriété de facturation:

- Pour conserver la propriété de facturation, mais modifier le type de votre abonnement, consultez: [Faites passer votre abonnement Azure à une autre offre](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Transfert des abonnements Visual Studio, Microsoft Partner Network (MPN) et Dev/Test paiement à l’utilisation](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Transférer la propriété de facturation des abonnements Accord Entreprise (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [FAQ Transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Résoudre les problèmes de transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)