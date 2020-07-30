---
title: Supprimer un canal privé Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431445"
---
# <a name="delete-a-teams-private-channel"></a>Supprimer un canal privé Teams

Microsoft a connaissance d’un problème lors de la suppression d’un canal privé Teams si les stratégies de rétention SharePoint sont activées pour le site SharePoint sous-jacent. Microsoft travaille à l’élaboration d’un correctif. En attendant, vous pouvez utiliser les solutions de contournement suivantes pour supprimer le canal privé.

**Exclure l’équipe ou la collection de sites de la stratégie de rétention SharePoint.**

1. Accédez au Portail d’administration Office 365 et sélectionnez **Afficher toutes** dans le volet de navigation gauche.
2. Sous **Centres d’administration**, accédez à **Sécurité et conformité** > **Protection contre la perte de données** > **stratégie**.
3. Identifiez les stratégies qui s’appliquent aux sites SharePoint et modifiez la stratégie de sorte que le site SharePoint pour l’équipe contenant le canal privé ne soit pas inclus dans la stratégie de rétention.
4. Enregistrez la stratégie.
    La prise en compte des paramètres de stratégie peut prendre jusqu’à 24 heures.
    Une fois le site exclu, vous pouvez supprimer le canal privé.  
    
Vous ***pouvez*** être en mesure de supprimer le canal privé à l’aide de Microsoft Teams sur votre appareil Android. 

Pour plus d’informations sur SharePoint, consultez [Impossible de supprimer des éléments dans SharePoint Online ou OneDrive Entreprise](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).