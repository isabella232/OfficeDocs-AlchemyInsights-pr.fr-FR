---
title: Activer la gestion des coûts
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003567"
---
# <a name="enable-cost-management"></a>Activer la gestion des coûts

**Que signifie « les coûts sont désactivés pour votre organisation » ?**

Les organisations utilisant Accord Entreprise (EA) ou des comptes contrat client Microsoft (MCA) peuvent désactiver l’accès aux informations de coût et aux informations de tarification.

Une fois qu’ils se connectent au portail Azure, ils peuvent utiliser les API de facturation pour obtenir par programme des factures (une fois que vous avez choisi) et des détails d’utilisation.

**Comment autoriser des utilisateurs supplémentaires à accéder aux factures**

1. Go to **Subscriptions blade** in Azure portal.
2. Sélectionnez **Factures,** puis **Accès aux factures.**
3. Activer l’accès, suivi de l’enregistrement des modifications, pour permettre aux utilisateurs dans des rôles d’étendue d’abonnement de télécharger des factures.

> [!NOTE]
> L’administrateur de compte peut également configurer l’envoi de factures par courrier électronique. Pour en savoir plus, [consultez Obtenir votre facture par courrier électronique.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Comment ajouter des utilisateurs au rôle Lecteur de facturation**

1. Go to **Subscriptions blade** in Azure portal.
2. Sélectionnez **Contrôle d’accès (IAM),** puis cliquez sur **Ajouter.**
3. Sélectionnez **Lecteur de facturation** dans la page Sélectionner **un** rôle.
4. Tapez l’e-mail de l’utilisateur que vous voulez inviter, puis cliquez sur **OK** pour envoyer l’invitation.
5. Suivez les instructions fournies dans l’e-mail d’invitation pour vous connecter en tant que lecteur de facturation. Pour plus d’informations, voir [Accorder l’accès à la facturation.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Documents recommandés**

- [Activer les vues DA et AO via le portail EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Coûts inclus dans la gestion des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Offres Microsoft Azure pris en charge](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Examiner les coûts dans l’analyse des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Fournir l’accès aux informations de facturation](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Vérifiez l’accès à un Contrat Client Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






