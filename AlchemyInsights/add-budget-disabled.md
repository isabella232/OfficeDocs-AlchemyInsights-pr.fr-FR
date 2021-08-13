---
title: Pourquoi le bouton Ajouter un budget est-il désactivé pour moi ?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954669"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Pourquoi le bouton Ajouter un budget est-il désactivé pour moi ?

Pour créer un budget, vous avez besoin de l’une des autorisations suivantes :

- Groupe de gestion, abonnement, étendues de groupe de ressources
- Collaborateur de gestion des coûts
- Propriétaire
- Collaborateur
- Enterprise Client uniquement : inscription, service, étendues de compte
- Administrateur d’inscription (définir le budget au niveau de l’étendue Inscription)
- Administrateur du service (définir le budget au niveau de l’étendue Service)
- Propriétaire du compte (définir le budget au niveau de l’étendue Compte)
- Contrat client moderne uniquement : compte de facturation, profil de facturation, étendues de section Facture
- Créateur d’abonnement Azure

**J’ai créé un budget lorsque mon coût pour le mois en cours était déjà sur le budget. Pourquoi n’ai-je pas reçu d’alerte ?**  
Si vous avez déjà dépassé un seuil de coût donné lorsque vous créez un budget, cette alerte ne se tirera pas. Une fois qu’un nouveau cycle commence, si vous enfreindez le seuil, l’alerte se produit.

**Quand dois-je m’attendre à recevoir une alerte après avoir dépassé l’un de mes seuils d’alerte budgétaire définis ?**  
Les budgets sont évalués toutes les 4 heures. Au moins 8 heures sont nécessaire pour que les données d’utilisation atteignent le système de budgets. Dans ce cas, le tir des alertes peut prendre jusqu’à 12 heures après le dépassement d’un seuil.

**Pourquoi le bouton Date de début est-il désactivé lorsque je sélectionne une période de réinitialisation mois ou mois de facturation ?**  
Les budgets sont alignés sur le mois calendaire actuel ou la période de facturation actuelle (dans le cas où le mois de facturation est sélectionné). Par conséquent, nous pré-remplissons cette valeur pour vous.

**Pourquoi ne vois-je pas de graphique de mes coûts dans l’expérience de création de budget ?**  
Nous avons besoin d’au moins 2 mois de données de coût avant de pouvoir restituer un graphique pour vous aider à créer un budget.

**Pourquoi ne puis-je pas définir un budget par rapport à un abonnement que je vient de créer ?**  
Après la création d’un abonnement, le traitement des données prend entre 24 et 48 heures avant de définir un budget par rapport à celui-ci.

**Ressources d’API budgétaires**

- [API Budgets v1 :](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)fournit des opérations pour créer et mettre à jour des budgets. À l’aide de l’API Budgets, vous pouvez définir un seuil budgétaire et configurer plusieurs alertes à l’approche de ce seuil. Les alertes peuvent déclencher un e-mail ou un groupe d’actions Azure pour effectuer l’automatisation. Remarque : le filtrage de cette API ne s’aligne pas sur le filtrage/dimensions de l’API de requête.
- [API Budgets v2 :](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)créer des budgets avec des fonctionnalités de filtrage des coûts plus élevées que la v1. Le filtrage s’aligne sur le contrat utilisé dans nos API Requête et Dimensions. Il s’agit de l’API de budgets recommandée à utiliser à l’avenir.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fournit des opérations pour obtenir des dimensions pris en charge pour votre utilisation sous une variété d’étendues. À l’aide de l’API Dimensions, vous pouvez récupérer une liste de dimensions qui peuvent être utilisées comme entrées pour générer des requêtes à l’aide de l’API de requête.
- [Requête :](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)fournit des opérations pour obtenir des données agrégées sur le coût et l’utilisation en fonction de la requête que vous fournissez. À l’aide de l’API de requête, vous pouvez spécifier le filtrage, le tri et le regroupement souhaités sur toutes les dimensions disponibles (accessibles à partir de l’API Dimensions).

**Coûts prévus**

**Pourquoi ne vois-je pas de prévisions pour mes coûts dans l’analyse des coûts ?**  
Il existe plusieurs raisons pour lesquelles la projection des prévisions est peut-être manquante pour vous dans l’analyse des coûts, certaines d’entre elles sont les suivantes :

1. Si vos données de coût ont moins de 10 jours, le graphique des prévisions ne se charge pas. Le modèle nécessite au moins 10 jours de données de coût récentes pour des projections précises
2. Si vous avez sélectionné des dates historiques, le graphique des prévisions ne sera pas visible. Veuillez sélectionner une plage de dates avec des dates futures pour le graphique des prévisions à afficher
3. Si votre compte possède plusieurs devises, le graphique des prévisions n’indique que les coûts de projet pour « Tous les coûts en USD »

**Pourquoi les prévisions ne changent-elles pas lorsque je modifie mes ressources ?**  
Le modèle de prévision nécessite quelques jours pour prendre en compte les modifications apportées au compte et ne permet pas d’effectuer des projections immédiates en fonction de la modification des ressources  
Pour les étapes plus importantes d’augmentation ou de diminution des ressources, le modèle prendra un peu plus de temps pour s’ajuster à ces modifications afin de tenir compte des anomalies

**Pourquoi mes prévisions augmentent-ils après avoir fait une réservation ou acheté sur Marketplace ?**  
Le modèle de prévision prend en compte votre « coût réel » et ne prend pas en compte l’utilisation et l’achat séparément. Pour un achat unique, le modèle réduit les projections au bout de 10 jours pour tenir compte de l’augmentation soudaine des coûts

**Je souhaite voir les prévisions pour une dimension unique (par exemple, Meter)**  
Les prévisions actuellement prend en charge les projections de coût total et non pour les mètres individuels. Par conséquent, lorsqu’elles sont « groupées par » une dimension, les projections sont pour le total de tous les éléments de la dimension.

**Documents Recommandés**

- [Qu’est-ce qu’Azure Cost Management ?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meilleures pratiques en matière de gestion des coûts Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analyser vos coûts et vos dépenses](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorer et analyser les coûts avec l’analyse des coûts](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management : tarification](https://azure.microsoft.com/services/cost-management/#pricing)
- [Examiner les coûts dans l’analyse des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Didacticiel vidéo : créer un budget dans le portail Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Conditions préalables à l’affichage et à la personnalisation des budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Créer et gérer des budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurer l’automatisation avec les groupes d’actions Azure et l’API Budgets](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utiliser des alertes de coût pour surveiller l’utilisation et les dépenses](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meilleures pratiques en matière de gestion des coûts](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vidéos de didacticiel**

- [Créer un budget dans le portail Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gérer les coûts avec l’API Budgets et les groupes d’actions](https://go.microsoft.com/fwlink/?linkid=2147038)