---
title: Facturation de l’achat d’instance réservée
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
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104018"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturation de l’achat d’instance réservée

L’achat de l’instance réservée est facturé selon le mode de paiement lié à l’abonnement que vous sélectionnez au moment de l’achat. Le type d’abonnement doit être un contrat d’entreprise (numéro d’offre : MS-AZR-0017P), Pay-as-You-Go (numéro d’offre : MS-AZR-0003P), Contrat client Microsoft ou CSP.

- Pour un abonnement d’entreprise, les frais sont déduits du solde de l’engagement monétaire de l’inscription ou facturés comme un sur-montant
- Pour l’abonnement Pay-As-You-Go, les frais sont facturés à la carte bancaire ou au mode de paiement par facture de l’abonnement.

**Annulation de la Réservation**

- **Libre-service:** Vous pouvez vous-même annuler ou échanger une instance réservée à l’aide du [Portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Sélectionnez la réservation, puis cliquez sur remboursement ou sur échange. Notez que vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation à échanger ou rembourser. L’accès à la réservation uniquement ne vous permet pas de procéder au remboursement ou à l’échange. Demandez au propriétaire de l’Ordre de Réservation de vous accorder l’accès de propriétaire à l’Ordre de Réservation
- **Stratégie d’échange :** Vous pouvez échanger une réservation pour une autre réservation du même type il n’y a **aucune pénalité** sur l’échange de la réservation. Le total de l’engagement avec une nouvelle réservation doit être supérieur à la somme du montant du remboursement de la réservation échangée et des prochains paiements mensuels (le cas échéant)
- **Stratégie de remboursement :** la somme du remboursement et les paiements futurs annulés ne peuvent pas dépasser 50 000$ USD dans une fenêtre de 12 mois successifs. Il n’y a **aucune pénalité pour l’instant** sur les remboursements, mais probablement à l’avenir.

**Exceptions :** L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis

- La prise en charge **API/PS/CLI** n’est pas disponible pour les annulations et remboursements [Les échanges et remboursements en libre-service pour les Réservations Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge

En savoir plus : [Comment les transactions](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) de retour et d’échange sont traitées En savoir plus : [Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) stratégies de remboursement Autres questions : Consulter les documents [d’instance réservées](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Echanger une instance réservée existante une instance (libre-service)**

Vous pouvez échanger une réservation avec une autre réservation du même type. Vous pouvez également rembourser une réservation, jusqu’à $50 000 USD par an, si vous n’en avez plus besoin. L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge. Vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation pour échanger ou rembourser une réservation existante.

Les étapes suivantes vous indiquent la procédure de la transaction

1.Connectez-vous à votre [portail Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Sélectionnez les réservations que vous souhaitez remboursement, puis cliquez sur **Exchange** 2.Sélectionnez le produit de machine automatique à acheter et tapez une quantité. Assurez-vous que le nouveau total d’achat est supérieur au total de retour [Déterminer la taille droite avant d’acheter](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Examiner et terminer la transaction

**Remboursement d’une instance réservée**

Pour rembourser une réservation, accédez à **Détails de la Réservation** puis cliquez sur **Remboursement.**

**Remboursement au prorata:**

**Pro-ration et exemples de conditions minimales requises pour le remboursement et l’échange** Exemple de réservation initiale :

- Vous achetez un RI valable pour un an à 120$ le 1er janvier
- Le 7 avril, vous voulez le remboursement ou l’échange de cette réservation
- La réservation étant en cours depuis 97 jours, vous obtiendrez (1-97/365) * 120$ comme remboursement. (c’est à dire, 88,1$). Il n’existe actuellement aucune pénalité pour les remboursements
- En cas d’échange, votre nouvel achat doit être supérieur à 88,1$
- Il n’y a pas de pénalité pour les remboursements actuellement

**Exemple de réservation de plan de facturation:**

- Vous achetez un RI valable pour un an à 10$ le par mois
- Le 7 avril, vous voulez le remboursement ou l’échange de cette réservation
- Etant donné que le dernier paiement a été effectué depuis 7 jours, vous obtiendrez (1-7/31) *10$ comme remboursement. (c’est à dire, 7,74$).
- Les remboursements futurs annulés sont 80$. Il n’existe actuellement aucune pénalité pour les remboursements
- Cette annulation déduit 87,74$ de la limite de remboursement de 50 000$
- En cas d’échange, la valeur totale de votre nouvel achat doit être supérieure à 87,74$

**Impossible de voir la facture pour la dernière période de facturation**

Voici quelques raisons possibles pour lesquelles vous ne voyez pas de facture :

- Vous avez un montant de crédit mensuel avec votre abonnement que vous n’avez pas dépassé ou vous avez une version d’essai gratuite. Une facture est générée uniquement lorsque vous devez payer
- Moins de 30 jours après le jour où vous vous êtes abonné à Azure
- La facture n’est pas encore générée. Attendre la fin de la période de facturation
- Si vous n’êtes pas l’administrateur de compte, il se peut que des factures plus anciennes ne soient pas disponibles.

**Télécharger votre facture à partir du portail Azure (.pdf)**

- Sélectionnez votre abonnement dans la page [Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) dans le portail Azure en tant [qu’utilisateur ayant accès aux factures](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Sélectionner **des factures**
- Cliquez sur **Télécharger la facture** pour afficher une copie de votre facture au format PDF. Si **Pas disponible** est indiqué, consultez [Pourquoi ne vois-je pas de facture pour la dernière période de facturation ?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Recevoir votre facture par courrier électronique (.pdf)**

- Sélectionnez votre abonnement dans la page [Abonnements.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Cliquez **sur Factures,** puis envoyez un e-mail à ma facture
- Cliquez **sur Accepter et** acceptez les termes. Vous devez vous abonner à chaque abonnement que vous possédez.

Remarque : si vous n’obtenez pas de message électronique après avoir suivi les étapes, assurez-vous que votre adresse de messagerie est correcte dans les préférences [de communication de votre profil](https://account.windowsazure.com/profile)

**Télécharger vos données d’utilisation à partir du portail Azure**

- Connectez-vous au [Centre de comptes Azure](https://account.windowsazure.com/Subscriptions) en tant [qu’administrateur de compte](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Sélectionnez l’abonnement pour lequel vous souhaitez obtenir la facture et les informations d’utilisation
- Sélectionner **l’historique de facturation**
- Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated
- Sélectionnez **Télécharger l’utilisation** pour télécharger les données d’utilisation quotidiennes en tant que fichier CSV. Si deux versions sont disponibles, téléchargez la version 2

Autres questions: [Visitez les documents sur les instances réservées](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documents Recommandés**

- [Informations de base sur la facturation](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre comment la remise d’instance réservée est appliquée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Télécharger ou afficher votre facture Azure et vos données d’utilisation quotidiennes](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre comment la remise d’instance réservée est appliquée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’utilisation des instances réservées pour votre abonnement À l’utilisation](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’utilisation des instances réservées pour Enterprise inscription](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows logiciels non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instances réservées dans le programme Fournisseur de solutions Cloud de partenaires](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)