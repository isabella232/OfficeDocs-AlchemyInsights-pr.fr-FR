---
title: 'Services de transfert : déplacer tous les services RDFE vers un autre abonnement'
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940052"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Services de transfert : déplacer tous les services RDFE vers un autre abonnement

**Déplacer des ressources**

Les ressources Azure peuvent être déplacées vers un autre abonnement Azure ou un autre groupe de ressources sous le même abonnement à l’aide du portail Azure, de Azure PowerShell, d’Azure CLI ou de l’API REST pour déplacer des ressources.

Avant de déplacer des ressources, voir :

- [Liste de vérification avant le déplacement des ressources](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Services qui peuvent être déplacés](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Comment valider le déplacement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Conseils de déplacement pour les services](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Pour déplacer des ressources existantes vers un autre groupe de ressources ou un autre abonnement, vous pouvez utiliser :

- [<mrk mtype="seg" mid="167">Portail Azure</mrk>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [API REST](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

[Didacticiel : Déplacer des ressources Azure vers un autre groupe de ressources ou un autre abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Résoudre les erreurs avec Azure Resource Manager**

Reportez-vous aux articles ci-dessous pour en savoir plus sur certaines erreurs de déploiement Azure courantes et recevoir des informations pour les résoudre. Si vous ne trouvez pas le code d’erreur pour votre erreur de déploiement, voir [Rechercher le code d’erreur.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Résoudre les erreurs de déploiement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Résoudre les problèmes de déplacement de ressources Azure vers un nouveau groupe de ressources ou un nouvel abonnement](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Notez que si vous souhaitez mettre à niveau votre abonnement Azure, par exemple en passant de la version gratuite à la version payante, vous devrez convertir votre abonnement.

- Pour mettre à niveau une version d’essai gratuite, voir Mettre à niveau votre version d’essai gratuite ou votre abonnement Microsoft Imagine Azure vers [Pay-As-You-Go.](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)
- Pour modifier un compte pay-as-you-go, voir Modifier votre abonnement [Azure Pay as-As-You-Go](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)en une autre offre.

**Pour ajouter ou associer un abonnement Azure à votre client Azure Active Directory client :**

1. Connectez-vous et sélectionnez l’abonnement que vous souhaitez utiliser dans la [page Abonnements dans le portail Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Sélectionnez **Modifier le répertoire.**
3. Examinez les avertissements qui s’affichent, puis sélectionnez **Modifier.**
4. Le répertoire est modifié pour l’abonnement et vous recevez un message de réussite.
5. Utilisez le *commutateur Directory* pour vous rendre dans votre nouveau répertoire. L’affiche peut prendre jusqu’à 10 minutes pour que tout s’affiche correctement.

**Documents Recommandés**

- [Transfert de la propriété d’un abonnement Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Déplacer des ressources vers un nouveau groupe de ressources ou un nouvel abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Gérer les ressources à l’aide du portail Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
