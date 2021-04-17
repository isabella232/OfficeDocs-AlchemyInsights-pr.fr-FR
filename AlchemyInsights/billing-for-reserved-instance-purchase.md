---
title: Facturation de l'achat d'instance réservée
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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820320"
---
# <a name="billing-for-reserved-instance-purchase"></a>Facturation de l'achat d'instance réservée

L'achat de l'instance réservée est facturé selon le mode de paiement lié à l'abonnement que vous sélectionnez au moment de l'achat. Le type d'abonnement doit être un contrat d'entreprise (numéro d'offre : MS-AZR-0017P), Pay-as-You-Go (numéro d'offre : MS-AZR-0003P), Contrat client Microsoft ou CSP.

- Pour un abonnement d'entreprise, les frais sont déduits du solde de l'engagement monétaire de l'inscription ou facturés comme un sur-montant
- Pour l'abonnement Pay-As-You-Go, les frais sont facturés à la carte bancaire ou au mode de paiement par facture de l'abonnement.

**Annulation de la réservation**

- **Libre-service :** Vous pouvez annuler ou échanger une instance réservée vous-même à l'aide [du portail Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Sélectionnez la réservation, puis cliquez sur remboursement ou échange. Notez que vous devez avoir accès au propriétaire sur la commande de réservation pour échanger ou remboursement. L'accès uniquement à la réservation ne vous permettra pas de procéder au remboursement ou à l'échange. Demandez au propriétaire de l'ordre de réservation de vous donner accès à la commande de réservation
- **Stratégie Exchange :** Vous pouvez échanger une réservation contre une autre réservation du même type : il n'y a aucune **pénalité sur** l'échange de réservation. L'engagement total avec la nouvelle réservation doit être supérieur à la somme du remboursement de la réservation échangée et aux paiements mensuels futurs (le cas échéant)
- **Politique de remboursement :** Le montant du remboursement et les paiements futurs annulés ne peuvent pas dépasser 50 000 $ USD dans une période de 12 mois. We are **currently not charge any penalty** on refunds but could charge it on future refunds

**Exceptions :** La fonctionnalité d'échange et d'annulation en libre-service n'est pas disponible pour les clients du contrat Entreprise pour le gouvernement américain

- La prise en charge **api/PS/CLI** n'est pas disponible pour l'annulation et rembourse les échanges et remboursements en [libre-service pour les réservations Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- La fonctionnalité d'échange et d'annulation en libre-service n'est pas disponible pour les clients du contrat Entreprise du gouvernement américain. D'autres types d'abonnements pour le gouvernement des États-Unis, notamment Pay-As-You-Go et CSP, sont pris en charge

En savoir plus : comment les transactions de retour et [d'échange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) sont traitées En savoir plus : [stratégies Exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) et remboursement Autres questions : consulter les documents [d'instance réservée](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange une instance réservée existante (libre-service)**

Vous pouvez échanger une réservation contre une autre réservation du même type. Vous pouvez également remboursement d'une réservation, jusqu'à 50 000 USD par an, si vous n'en avez plus besoin. La fonctionnalité d'échange et d'annulation en libre-service n'est pas disponible pour les clients du contrat Entreprise du gouvernement américain. D'autres types d'abonnements pour le gouvernement des États-Unis, notamment Pay-As-You-Go et CSP, sont pris en charge. Vous devez avoir accès au propriétaire sur la commande de réservation pour échanger ou remboursement d'une réservation existante.

Les étapes suivantes guident la procédure pour effectuer la transaction

1.Connectez-vous à votre [portail Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Sélectionnez les réservations à remboursement, puis cliquez sur **Exchange** 2.Sélectionnez le produit de machine automatique à acheter et tapez une quantité. Assurez-vous que le nouveau total d'achat est supérieur au total de retour [Déterminer la taille droite avant d'acheter](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3.Examiner et terminer la transaction

**Remboursement d'une instance réservée**

Pour remboursement d'une réservation, consultez **les détails de la** réservation et cliquez sur **Remboursement**

**Remboursement au pro-taux :**

**Exemples de pro-ration et de conditions minimales requises pour le remboursement et l'échange** Exemple de réservation initiale :

- Vous achetez une ir pour une période d'un an pour 120 dollars le 1er janvier
- Le 7 avril, vous souhaitez remboursement ou échanger cette réservation
- Étant donné que la réservation est en ligne depuis 97 jours, vous recevez (1-97/365) * 120 $ de retour. (c'est-à-dire, 88,1 dollars). Il n'existe actuellement aucune pénalité sur les remboursements
- En cas d'échange, votre nouvel achat doit être supérieur à 88,1 dollars.
- Il n'y a aucune pénalité pour les remboursements actuellement

**Exemple de réservation de plan de facturation :**

- Vous achetez une ri pour une période d'un an de 10 dollars par mois
- Le 7 avril, vous souhaitez remboursement ou échanger cette réservation
- Étant donné que le dernier paiement a eu lieu 7 jours, vous recevez (1-7/31) * 10 $ de retour. (c'est-à-dire, 7,74 $)
- Les paiements futurs annulés sont de 80 $. Il n'existe actuellement aucune pénalité sur les remboursements
- Cette annulation déduit 87,74 $ de la limite de remboursement de 50 000 $
- En cas d'échange, la valeur totale du nouvel achat doit être supérieure à 87,74 dollars.

**Impossible de voir la facture pour la dernière période de facturation**

Voici quelques raisons possibles pour lesquelles vous ne voyez pas de facture :

- Vous avez un montant de crédit mensuel avec votre abonnement que vous n'avez pas dépassé ou vous avez une version d'essai gratuite. Une facture est générée uniquement lorsque vous devez payer
- Moins de 30 jours après le jour où vous vous êtes abonné à Azure
- La facture n'est pas encore générée. Attendre la fin de la période de facturation
- Si vous n'êtes pas l'administrateur de compte, il se peut que les anciennes factures ne soient pas disponibles.

**Télécharger votre facture à partir du portail Azure (.pdf)**

- Sélectionnez votre abonnement dans la page [Abonnements](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) dans le portail Azure en tant [qu'utilisateur ayant accès aux factures](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Sélectionner **des factures**
- Cliquez sur **Télécharger la facture** pour afficher une copie de votre facture au format PDF. Si elle indique **Non disponible,** consultez pourquoi une facture pour la dernière période de facturation ne [s'affiche-t-elle pas ?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Recevoir votre facture par courrier électronique (.pdf)**

- Sélectionnez votre abonnement dans la page [Abonnements.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Cliquez **sur Factures,** puis envoyez un e-mail à ma facture
- Cliquez **sur Accepter et** acceptez les termes. Vous devez vous abonner à chaque abonnement que vous possédez.

Remarque : si vous n'obtenez pas de message électronique après avoir suivi les [étapes,](https://account.windowsazure.com/profile) assurez-vous que votre adresse de messagerie est correcte dans les préférences de communication de votre profil.

**Télécharger vos données d'utilisation à partir du portail Azure**

- Connectez-vous au [Centre de comptes Azure](https://account.windowsazure.com/Subscriptions) en tant [qu'administrateur de compte](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Sélectionnez l'abonnement pour lequel vous souhaitez obtenir la facture et les informations d'utilisation
- Sélectionner **l'historique de facturation**
- Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated
- Sélectionnez **Télécharger l'utilisation** pour télécharger les données d'utilisation quotidiennes en tant que fichier CSV. Si deux versions sont disponibles, téléchargez la version 2

Autres questions : Consulter [les documents sur les instances réservées](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Documents recommandés**

- [Informations de base sur la facturation](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre comment la remise d'instance réservée est appliquée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Télécharger ou afficher votre facture Azure et vos données d'utilisation quotidiennes](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre comment la remise d'instance réservée est appliquée](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l'utilisation des instances réservées pour votre abonnement À l'utilisation](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comprendre l'utilisation des instances réservées pour votre inscription entreprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Coûts logiciels Windows non inclus dans les instances réservées](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Instances réservées dans le programme Fournisseur de solutions Cloud de l'Espace partenaires](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)