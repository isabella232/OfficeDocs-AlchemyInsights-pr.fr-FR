---
title: Pourquoi le bouton Ajouter un budget est-il désactivé ?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769588"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Pourquoi le bouton Ajouter un budget est-il désactivé ?

Pour créer un budget, vous avez besoin de l’une des autorisations suivantes :

- Groupes d’administration, abonnements, étendues de groupes de ressources
- Collaborateur de gestion des coûts
- Propriétaire
- Collaborateur
- Client entreprise uniquement : inscriptions, service, étendues de compte
- Administrateur d’inscriptions (définir le budget à l’étendue de l’enregistrement)
- Administrateur de service (définir le budget au niveau de l’étendue du service)
- Propriétaire du compte (définir le budget au niveau de l’étendue du compte)
- Contrat de client moderne uniquement : compte de facturation, profil de facturation, étendues de section de facture
- Créateur d’abonnement Azure

**J’ai créé un budget lorsque mon coût pour le mois en cours était déjà dépassé. Pourquoi ne puis-je pas recevoir d’alerte ?**  
Si vous avez déjà dépassé un seuil de coût donné lorsque vous créez un budget pour lequel l’alerte ne se déclenche pas. Une fois qu’un nouveau cycle commence, si vous violez le seuil, l’alerte est déclenchée.

**Quand dois-je m’attendre à recevoir une alerte après que j’ai dépassé l’un des seuils d’alerte budgétaire définis ?**  
Les budgets sont évalués toutes les 4 heures. Il faut au minimum 8 heures pour que les données d’utilisation atteignent le système des budgets. Dans ce cas, les alertes peuvent prendre jusqu’à 12 heures pour se déclencher une fois que vous avez dépassé le seuil autorisé.

**Pourquoi le bouton date de début est-il désactivé lorsque je sélectionne un mois ou une période de réinitialisation du mois de facturation ?**  
Les budgets sont alignés sur le mois civil actuel ou sur la période de facturation actuelle (dans le cas où le mois de facturation est sélectionné). Par conséquent, nous prévoyons cette valeur pour vous.

**Pourquoi ne puis-je pas voir un graphique de mes coûts dans l’expérience de création de budget ?**  
Nous avons besoin d’un minimum de 2 mois de données de coûts avant de pouvoir afficher un graphique pour vous aider à la création de budget.

**Pourquoi ne puis-je pas définir un budget par rapport à un abonnement que je viens de créer ?**  
Après la création d’un abonnement, les données prennent 24-48 heures avant de définir un budget.

**Ressources de l’API de budget**

- [API budgets v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): fournit des opérations pour créer et mettre à jour des budgets. À l’aide de l’API budgets, vous pouvez définir un seuil budgétaire et configurer plusieurs alertes pour les déclencher à mesure que vous approchez ce seuil. Les alertes peuvent déclencher un courrier électronique ou un groupe d’actions Azure pour effectuer l’automatisation. Remarque : le filtrage de cette API ne s’aligne pas avec le filtrage/les dimensions de l’API de requête.
- [API de budgets v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): créez des budgets avec des capacités de filtrage des coûts supérieures à la version v1. Le filtrage s’aligne sur le contrat utilisé dans nos API requête et dimensions. Il s’agit de l’API de budgets recommandés pour utiliser l’avenir.
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): fournit des opérations pour obtenir des dimensions prises en charge pour votre utilisation sous diverses étendues. À l’aide de l’API dimensions, vous pouvez récupérer une liste de dimensions pouvant être utilisées comme entrées pour générer des requêtes à l’aide de l’API de requête.
- [Requête](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): fournit des opérations pour obtenir des données agrégées et des données d’utilisation en fonction de la requête que vous fournissez. À l’aide de l’API de requête, vous pouvez spécifier le filtrage, le tri et le regroupement souhaités sur toutes les dimensions disponibles (accessibles à partir de l’API de dimensions).

**Coûts prévus**

**Pourquoi ne puis-je pas voir les prévisions pour mes coûts dans l’analyse des coûts ?**  
Il existe plusieurs raisons pour lesquelles la prévision de prévision peut être manquante pour vous dans l’analyse des coûts, dont certaines sont les suivantes :

1. Si vos données de coût sont datant de moins de 10 jours, le graphique de prévision ne sera pas chargé. Le modèle nécessite au moins 10 jours de données de coût récentes pour les prévisions précises
2. Si vous avez sélectionné dates d’historique, le graphique de prévision n’est pas visible. Sélectionnez une plage de dates pour les dates futures pour le graphique des prévisions à afficher.
3. Si votre compte comporte plusieurs devises, le graphique de prévision contiendra uniquement les coûts « tous les coûts dans USD ».

**Pourquoi la prévision n’est-elle pas modifiée lorsque je modifie mes ressources ?**  
Le modèle de prévision requiert quelques jours pour tenir compte des modifications apportées au compte et ne fait pas de projections immédiates en fonction des modifications apportées aux ressources.  
Pour les grandes étapes de l’augmentation ou de la diminution des ressources, le modèle prendra un peu plus de temps pour tenir compte des anomalies.

**Pourquoi mes prévisions augmentent-elles après avoir effectué une réservation ou un achat de marché ?**  
Le modèle de prévision considère votre « coût réel » et ne tient pas compte de l’utilisation et de l’achat séparément. Pour un achat unique, le modèle réduira les prévisions au bout de 10 jours pour tenir compte de l’augmentation soudaine des coûts.

**Je souhaite afficher les prévisions pour une seule dimension (par exemple, Comptage**  
La prévision prend actuellement en charge les prévisions de coûts totales et non pour les compteurs individuels. Par conséquent, quand « groupé par » une dimension, les projections seront pour le total de tous les éléments de la dimension.

**Documents recommandés**

- [Qu’est-ce que la gestion des coûts Azure ?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meilleures pratiques en matière de gestion des coûts Azure](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analyser vos dépenses et dépenses](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Explorer et analyser les coûts liés à l’analyse des coûts](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Gestion des coûts Azure : tarification](https://azure.microsoft.com/services/cost-management/#pricing)
- [Examiner les coûts dans l’analyse des coûts](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Didacticiel vidéo : créer un budget dans le portail Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Conditions préalables à l’affichage et à la personnalisation des budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Créer et gérer des budgets](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Configurer l’automatisation avec les groupes d’actions Azure et l’API de budgets](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Utiliser des alertes de coûts pour surveiller l’utilisation et les dépenses](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Meilleures pratiques en matière de gestion des coûts](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Vidéos du didacticiel**

- [Créer un budget dans le portail Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Gérer les coûts avec l’API budgets et les groupes d’actions](https://go.microsoft.com/fwlink/?linkid=2147038)