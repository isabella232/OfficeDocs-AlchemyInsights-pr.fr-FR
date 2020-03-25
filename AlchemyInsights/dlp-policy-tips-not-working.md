---
title: Les conseils de stratégie DLP ne fonctionnent pas
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932584"
---
# <a name="dlp-policy-tip-issues"></a>Problèmes de Conseil de stratégie DLP

**Important**: de nombreux clients SharePoint Online et OneDrive exécutent des applications métiers critiques contre le service exécuté en arrière-plan. Ces applications incluent la migration de contenu, la protection contre la perte de données (DLP) et les solutions de sauvegarde. Pendant ces périodes inégalées, nous mettons tout en œuvre pour garantir un haut niveau de disponibilité et de fiabilité des services SharePoint Online et OneDrive à vos utilisateurs qui comptent plus que jamais sur le service dans les scénarios de travail à distance.

Dans le cadre de cet objectif, nous avons implémenté des limitations plus strictes pour les applications d’arrière-plan (solutions de migration, de protection contre la perte de données et de sauvegarde) pendant les heures de la semaine. Selon toute probabilité, ces applications offriront un débit très limité pendant ces horaires. Toutefois, pendant les heures de soirée et de week-end pour la région, le service sera prêt à traiter un volume considérablement plus important de demandes d’applications d’arrière-plan.

**Conseils de stratégie DLP**

Lorsque vous utilisez des **stratégies DLP**, les utilisateurs peuvent être avertis d’une violation de stratégie à l’aide de **conseils de stratégie**. Les administrateurs peuvent configurer des conseils de stratégie à afficher pendant le test de leur stratégie DLP ou lorsque la stratégie est en mode d’application complète.
  
Pour configurer des conseils de stratégie sur votre stratégie DLP dans le centre de sécurité et de conformité en mode d’application complète, procédez comme suit :
  
- Assurez-vous que les conseils de stratégie ont été **activés** sur la règle DLP en suivant les étapes [ci-dessous](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Vérifiez que votre **contenu correspond** à ce qui est **requis** pour déclencher la règle décrite dans cet article [ici](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Les conseils de stratégie sont affichés dans OWA et Outlook. Toutefois, lorsque vous utilisez **Outlook 2013 ou une version ultérieure**, les conseils de stratégie s’affichent uniquement dans certaines conditions. Ces conditions sont répertoriées ci-dessous : [conditions prises en charge pour Outlook 2013 ou version ultérieure pour l’affichage des conseils de stratégie](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Pour plus d’informations sur les conseils de stratégie DLP, voir : [afficher les conseils de stratégie pour les stratégies DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  