---
title: Transférer la propriété de facturation Azure
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840606"
---
# <a name="transfer-azure-billing-ownership"></a>Transférer la propriété de facturation Azure

Connectez-vous au [portail Azure](https://portal.azure.com/) comme administrateur du compte de facturation qui contient l’abonnement que vous voulez transférer. Si vous ne savez pas si vous êtes administrateur, ou si vous avez besoin de déterminer qui l’est, voir [Déterminer l’administrateur de facturation d’un compte](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Recherchez sur **Gestion des coûts + Facturation**.
- Sélectionnez **Abonnements** dans le volet gauche. Selon l’accès, vous devrez peut-être sélectionner une étendue de facturation, puis **Abonnements** ou **Abonnements Azure**.
- Sélectionnez **Transférer la propriété de facturation** pour l’abonnement que vous voulez transférer.
- Entrez l’adresse e-mail d’un utilisateur qui est un administrateur de facturation du compte qui sera le nouveau propriétaire de l’abonnement, puis sélectionnez **envoyer une demande de transfert**
- L’utilisateur reçoit un e-mail contenant des instructions pour examiner votre demande de transfert. Pour approuver la demande de transfert, l’utilisateur sélectionne le lien dans l’email et suit les instructions.

**Remarque**  : si vous transférez la propriété de facturation à un compte d’utilisateur dans un autre client Azure AD, toutes les attributions de [contrôle d’accès en fonction du rôle (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) servant à gérer les ressources dans l’abonnement sont supprimées définitivement. Seul le nouveau propriétaire peut accéder à la gestion des ressources dans l’abonnement. Pour plus d’informations, consultez [transfert d’un abonnement à un utilisateur dans un autre client Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documents recommandés**

- [Transférer la propriété de facturation d’un abonnement Azure vers un autre compte](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [À propos du transfert de propriété de facturation pour un abonnement Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transfert des abonnements Visual Studio, Microsoft Partner Network (MPN) et Dev/Test avec paiement à l’utilisation](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [FAQ Transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Résoudre les problèmes de transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
