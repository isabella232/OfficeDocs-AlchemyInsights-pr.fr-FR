---
title: Facturation de l’achat d’instance Réservée
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816005"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturation de l’achat d’instance Réservée

L’achat de l’instance réservée est débitée du mode de paiement associé à l’abonnement que vous sélectionnez au moment de l’achat. Le type d’abonnement doit être un accord d’entreprise (numéro d’offre : MS-AZR-0017P), Paiement à l’Utilisation (numéro d’offre : MS-AZR-0003P), Contrat Client Microsoft ou fournisseur de solutions Microsoft Cloud.

- Pour un abonnement d’entreprise, les frais sont déduits du solde de l’engagement financier de l’inscription ou de la facturation de dépassement.
- Pour les abonnements au Paiement à l’Utilisation, les frais sont facturés sur la carte de crédit ou le mode de paiement de la facture à l’abonnement.

**Annulation de la Réservation**

- **Libre-service:** Vous pouvez vous-même annuler ou échanger une instance réservée à l’aide du [Portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Sélectionnez la réservation, puis cliquez sur remboursement ou sur échange. Notez que vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation à échanger ou rembourser. L’accès à la réservation uniquement ne vous permet pas de procéder au remboursement ou à l’échange. Demandez au propriétaire de l’Ordre de Réservation de vous accorder l’accès de propriétaire à l’Ordre de Réservation
- **Stratégie d’échange :** Vous pouvez échanger une réservation pour une autre réservation du même type il n’y a **aucune pénalité** sur l’échange de la réservation. Le total de l’engagement avec une nouvelle réservation doit être supérieur à la somme du montant du remboursement de la réservation échangée et des prochains paiements mensuels (le cas échéant)
- **Stratégie de remboursement :** la somme du remboursement et les paiements futurs annulés ne peuvent pas dépasser 50 000$ USD dans une fenêtre de 12 mois successifs. Il n’y a **aucune pénalité pour l’instant** sur les remboursements, mais probablement à l’avenir.

**Exceptions :** L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis

- La prise en charge **API/PS/CLI** n’est pas disponible pour les annulations et remboursements [Les échanges et remboursements en libre-service pour les Réservations Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge

Pour plus d’informations [, consultez la procédure de traitement des transactions de retour et d’Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) en savoir plus sur les autres questions relatives aux [stratégies Exchange et de remboursement](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) : [visiter documents d’instance réservés](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Echanger une instance réservée existante une instance (libre-service)**

Vous pouvez échanger une réservation avec une autre réservation du même type. Vous pouvez également rembourser une réservation, jusqu’à $50 000 USD par an, si vous n’en avez plus besoin. L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge. Vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation pour échanger ou rembourser une réservation existante.

Les étapes suivantes vous indiquent la procédure de la transaction

1. Connectez-vous à votre [portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Sélectionnez les réservations que vous souhaitez rembourser et cliquez sur **Exchange** 2. Sélectionnez le produit VM que vous souhaitez acheter et tapez une quantité. Assurez-vous que le total des nouveaux achats est supérieur au total de retour [détermine la taille appropriée avant l’achat](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. Vérifiez et terminez la transaction.

**Remboursement d’une instance réservée**

Pour rembourser une réservation, accédez à **Détails de la Réservation** puis cliquez sur **Remboursement.**

**Remboursement au prorata:**

**Exemples de conditions requises pour le remboursement et l’échange d’un besoin minimal** Exemple de réservation avant :

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

**Impossible d’afficher la facture pour la dernière période de facturation**

Voici quelques raisons pour lesquelles il est possible que vous ne voyez pas de facture :

- Vous avez un crédit mensuel avec votre abonnement que vous n’avez pas dépassé ou que vous disposez d’une version d’évaluation gratuite. Une facture n’est générée que lorsque vous devez de l’argent
- Il s’agit de moins de 30 jours à compter du jour auquel vous êtes abonné à Azure
- La facture n’est pas encore générée. Attendre la fin de la période de facturation
- Si vous n’êtes pas l’administrateur de compte, les factures plus anciennes ne seront peut-être pas disponibles.

**Télécharger votre facture à partir du portail Azure (. pdf)**

- Sélectionnez votre abonnement dans la page [abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) du portail Azure en tant qu' [utilisateur ayant accès aux factures](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Sélectionner les **factures**
- Cliquez sur **Télécharger la facture** pour afficher une copie de votre facture PDF. Si elle indique **non disponible** , consultez [la rubrique pourquoi ne vois-je pas de facture pour la dernière période de facturation ?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Recevoir votre facture par e-mail (. pdf)**

- Sélectionnez votre abonnement dans la page [abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) . Cliquez sur **factures** , envoyer ma facture par courrier électronique
- Cliquez **sur accepter et** acceptez les termes. Vous devrez choisir un abonnement pour chaque abonnement que vous possédez

Remarque : Si vous n’obtenez pas de message électronique après avoir suivi les étapes, vérifiez que votre adresse de courrier est correcte dans les [Préférences de communication de votre profil](https://account.windowsazure.com/profile) .

**Télécharger vos données d’utilisation à partir du portail Azure**

- Connectez-vous au [Centre de comptes Azure](https://account.windowsazure.com/Subscriptions) en tant qu' [administrateur de compte](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) .
- Sélectionnez l’abonnement pour lequel vous souhaitez obtenir les informations de facturation et d’utilisation.
- Sélectionner **l’historique de facturation**
- Sélectionnez **View Current Statement (afficher le relevé actuel** ) pour afficher une estimation de vos frais au moment où l’estimation a été générée.
- Sélectionnez **Télécharger l’utilisation** pour télécharger les données d’utilisation quotidiennes sous forme de fichier CSV. Si deux versions sont disponibles, téléchargez la version 2.

Autres questions: [Visitez les documents sur les instances réservées](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documents Recommandés**

- [Principes de base de la facturation](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’application de la remise de l’instance réservée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Télécharger ou afficher votre facture Azure facturation et les données d’utilisation journalière](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’application de la remise de l’instance réservée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’utilisation des instances réservées pour votre abonnement paiement en tant que](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l’utilisation de l’instance réservée pour votre entreprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Coûts logiciels Windows non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instances réservées dans le programme de fournisseur de solutions Cloud (CSP) partenaire](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)