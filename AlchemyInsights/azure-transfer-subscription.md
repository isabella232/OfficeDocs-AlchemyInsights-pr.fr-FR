---
title: Transférer la propriété de facturation Azure
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036094"
---
# <a name="transfer-azure-billing-ownership"></a>Transférer la propriété de facturation Azure

Connectez-vous au [portail Azure](https://portal.azure.com/) comme administrateur du compte de facturation qui contient l’abonnement que vous voulez transférer. Si vous ne savez pas si vous êtes administrateur, ou si vous avez besoin de déterminer qui l’est, voir [Déterminer l’administrateur de facturation d’un compte](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Recherchez _Gestion des coûts + Facturation_.
1. Sélectionnez **Abonnements** dans le volet gauche. Selon l’accès, vous devrez peut-être sélectionner une étendue de facturation, puis **Abonnements** ou **Abonnements Azure**.
1. Sélectionnez **Transférer la propriété de facturation** pour l’abonnement que vous voulez transférer.
1. Entrez l’adresse e-mail d’un utilisateur qui est un administrateur de facturation du compte qui sera le nouveau propriétaire de l’abonnement, puis sélectionnez **envoyer une demande de transfert**.
1. L’utilisateur reçoit un e-mail contenant des instructions pour examiner votre demande de transfert. Pour approuver la demande de transfert, l’utilisateur sélectionne le lien dans l’email et suit les instructions.

Veuillez noter que si vous transférez la propriété de facturation à un compte d’utilisateur dans un autre client Azure AD, toutes les attributions de [contrôle d’accès en fonction du rôle (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) servant à gérer les ressources dans l’abonnement sont supprimées définitivement. Seul le nouveau propriétaire peut accéder à la gestion des ressources dans l’abonnement. Pour plus d’informations la modification du répertoire, consultez [transfert d’un abonnement à un utilisateur dans un autre client Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Impact important sur vos factures**_  : si vous avez transféré la propriété de facturation d’un abonnement Azure, vos frais sont classés au prorata. Vous pouvez accéder aux factures en procédant comme suit :  

1. Sélectionnez votre abonnement dans la  [page Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) dans le portail Azure comme [un utilisateur ayant accès aux factures](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), puis sélectionnez **Factures**.
1. Cliquez sur  **Télécharger la facture**  pour afficher une copie de votre facture au format PDF. Si  _Pas disponible_ est indiqué, consultez  [Pourquoi ne vois-je pas de facture pour la dernière période de facturation ?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Vous pouvez également afficher votre utilisation quotidienne en cliquant sur la **période de facturation**. Pour obtenir une version PDF de votre facture et une copie de votre fichier d’utilisation quotidienne détaillée (.CSV). Pour plus d’informations, consultez  [Obtenir les données de facturation et d’utilisation](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Documents recommandés**

- [Transférer la propriété de facturation d’un abonnement Azure vers un autre compte](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [À propos du transfert de propriété de facturation pour un abonnement Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Transfert des abonnements Visual Studio, Microsoft Partner Network (MPN) et Dev/Test avec paiement à l’utilisation](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [FAQ Transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Résoudre les problèmes de transfert de propriété](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
