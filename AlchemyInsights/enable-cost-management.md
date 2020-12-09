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
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599061"
---
# <a name="enable-cost-management"></a>Activer la gestion des coûts

**Que signifie « les coûts sont désactivés pour votre organisation » ?**

Les organisations qui utilisent des comptes accord entreprise (EA) ou Microsoft client Agreement (MCA) peuvent désactiver l’accès aux informations de coûts et aux informations de tarification.

Une fois connecté au portail Azure, il peut utiliser les API de facturation pour obtenir des factures (par programme) et des détails sur l’utilisation.

**Procédure autoriser les utilisateurs supplémentaires à accéder aux factures**

1. Accédez à **Blade d’abonnements** dans le portail Azure.
2. Sélectionnez **factures** , puis **accès aux factures**.
3. Activez l’accès, suivi de l’enregistrement des modifications, pour permettre aux utilisateurs de rôles d’étendue d’abonnement de télécharger des factures.

> [!NOTE]
> L’administrateur de compte peut également configurer de façon à ce que les factures soient envoyées par courrier électronique. Pour en savoir plus, consultez [la rubrique obtenir votre facture dans un courrier électronique](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Comment ajouter des utilisateurs au rôle de lecteur de facturation**

1. Accédez à **Blade d’abonnements** dans le portail Azure.
2. Sélectionnez **contrôle d’accès (IAM)** , puis cliquez sur **Ajouter**.
3. Sélectionnez **lecteur de facturation** dans la page **Sélectionner un rôle** .
4. Tapez l’adresse de messagerie de l’utilisateur que vous souhaitez inviter, puis cliquez sur **OK** pour envoyer l’invitation.
5. Suivez les instructions fournies dans le message d’invitation pour vous connecter en tant que lecteur de facturation. Pour plus d’informations, consultez la rubrique [accorder l’accès à la facturation](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Documents recommandés**

- [Activer les affichages DA et AO via le portail EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Coûts inclus dans la gestion des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Offres Microsoft Azure prises en charge](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Examiner les coûts dans l’analyse des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Donner accès aux informations de facturation](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Vérifier l’accès à un accord client Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






