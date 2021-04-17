---
title: Annulation de la Réservation
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819690"
---
# <a name="cancelling-reservation"></a>Annulation de la Réservation

- **Libre-service:** Vous pouvez vous-même annuler ou échanger une instance réservée à l’aide du [Portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Sélectionnez la réservation, puis cliquez sur remboursement ou sur échange. Notez que vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation à échanger ou rembourser. L’accès à la réservation uniquement ne vous permet pas de procéder au remboursement ou à l’échange. Demandez au propriétaire de l’Ordre de Réservation de vous accorder l’accès de propriétaire à l’Ordre de Réservation
- **Stratégie d’échange :** Vous pouvez échanger une réservation pour une autre réservation du même type il n’y a **aucune pénalité** sur l’échange de la réservation. Le total de l’engagement avec une nouvelle réservation doit être supérieur à la somme du montant du remboursement de la réservation échangée et des prochains paiements mensuels (le cas échéant)
- **Stratégie de remboursement :** la somme du remboursement et les paiements futurs annulés ne peuvent pas dépasser 50 000$ USD dans une fenêtre de 12 mois successifs. Il n’y a **aucune pénalité pour l’instant** sur les remboursements, mais probablement à l’avenir.  
    **Exceptions :** L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis
- La prise en charge **API/PS/CLI** n’est pas disponible pour les annulations et remboursements [Les échanges et remboursements en libre-service pour les Réservations Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge

En savoir plus sur le: [Traitement des transactions de retour et d’échange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
En savoir plus sur : [Les stratégies de remboursement et d’échange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Autres questions: [Visitez les documents sur les instances réservées](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Echanger une instance réservée existante une instance (libre-service)**

Vous pouvez échanger une réservation avec une autre réservation du même type. Vous pouvez également rembourser une réservation, jusqu’à $50 000 USD par an, si vous n’en avez plus besoin. L’échange libre-service et la fonctionnalité d’annulation ne sont pas disponibles pour les clients soumis à l’Accord Entreprise du Gouvernement des États-Unis. D’autres types d’abonnements du Gouvernement des États-Unis, notamment le Paiement à l’Utilisation et le CSP sont pris en charge. Vous devez disposer d’un accès de propriétaire sur l’Ordre de Réservation pour échanger ou rembourser une réservation existante.

Les étapes suivantes vous indiquent la procédure de la transaction

1. Connectez-vous à votre [Portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Sélectionnez les réservations que vous voulez rembourser, puis cliquez sur **Echanger**
2. Sélectionnez le produit VM que vous voulez acheter, puis saisissez une quantité. Assurez-vous que le total des nouveaux achats est supérieur au total des retours [Déterminer la taille appropriée avant l’achat](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Consultez et terminez la transaction

**Remboursement d’une instance réservée**

Pour rembourser une réservation, accédez à **Détails de la Réservation** puis cliquez sur **Remboursement.**

**Remboursement au prorata:**

**Exemples de remboursement et d’échange au prorata et à condition minimale**  
Exemple de réservation préalable:

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

**Documents Recommandés**

- [Traitement des transactions de retour et d’échange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Les stratégies d’Echange et de Remboursement](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)