---
title: 'Transfer Services : déplacer tous les services RDFE vers un autre abonnement'
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681461"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services : déplacer tous les services RDFE vers un autre abonnement

**Déplacer des ressources**

Les ressources Azure peuvent être déplacées vers un autre abonnement ou groupe de ressources Azure sous le même abonnement à l’aide du portail Azure, d’Azure PowerShell, de l’interface CLI Azure ou de l’API REST pour déplacer des ressources.

Avant de pouvoir déplacer des ressources, voir :

- [Liste de vérification avant de transférer des ressources](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Services pouvant être déplacés](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comment valider le déplacement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Conseils de déplacement pour les services](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pour déplacer des ressources existantes vers un autre groupe de ressources ou abonnement, vous pouvez utiliser les éléments suivants :

- [Portail Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Interface de commande de commande Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Didacticiel : [déplacer des ressources Azure vers un autre groupe de ressources ou abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Résoudre les erreurs avec Azure Resource Manager**

Consultez les articles ci-dessous pour en savoir plus sur les erreurs de déploiement Azure courantes et recevoir des informations pour les résoudre. Si vous ne trouvez pas le code d’erreur de votre erreur de déploiement, reportez-vous à la rubrique [Rechercher le code d’erreur](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Résoudre les erreurs de déploiement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Résoudre les problèmes de transfert de ressources Azure vers un nouveau groupe de ressources ou un nouvel abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Notez que si vous souhaitez mettre à niveau votre abonnement Azure, par exemple pour passer de la version gratuite à payer en tant que vous-même, vous devrez convertir votre abonnement.

- Pour mettre à niveau une version d’évaluation gratuite, consultez [la rubrique mise à niveau de votre version d’évaluation gratuite ou de votre abonnement Microsoft imagine Azure pour payer en tant que vous-même](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Pour modifier un compte facturé en tant que, consultez [la rubrique change your Azure pay-as-do-on-by Subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**Pour ajouter ou associer un abonnement Azure à votre client Azure Active Directory :**

1. Connectez-vous et sélectionnez l’abonnement que vous souhaitez utiliser à partir de la [page abonnements dans le portail Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Sélectionnez **changer de répertoire**.
3. Examinez les avertissements qui s’affichent, puis sélectionnez **modifier**.
4. Le répertoire est modifié pour l’abonnement et vous obtiendrez un message de réussite.
5. Utilisez le sélecteur d' *Annuaire* pour accéder à votre nouveau répertoire. L’affichage correct de tous les éléments peut prendre jusqu’à 10 minutes.

**Documents recommandés**

- [Transfert de la propriété d’un abonnement Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Déplacer des ressources vers un nouveau groupe de ressources ou un nouvel abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gérer les ressources à l’aide du portail Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
