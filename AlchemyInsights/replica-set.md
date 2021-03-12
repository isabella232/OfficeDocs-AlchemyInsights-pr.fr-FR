---
title: Jeu de réplicas
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716270"
---
# <a name="replica-set"></a>Jeu de réplicas

AADDS est également appelé domaine géré. Il s’agit en fait de deux contrôleurs de domaine qui sont exécutés et gérés par le back-end. Les deux DCS incluent un DC principal et un DC de réplication. Les sauvegardes dans AADDS (domaine géré) sont un processus automatisé géré par la plateforme Azure. En cas de problème avec votre domaine géré, le support Azure peut vous aider à restaurer à partir d’une sauvegarde.

Vous créez chaque jeu de réplicas dans un réseau virtuel. Chaque réseau virtuel doit être homologue à tous les autres réseaux virtuels qui hébergent le jeu de réplicas d’un domaine géré. Cette configuration crée une topologie de réseau de maillage qui prend en charge la réplication d’annuaires. Un réseau virtuel peut prendre en charge plusieurs jeux de réplicas, à condition que chaque jeu de réplicas se trouve dans un sous-réseau virtuel différent.

Pour plus d’informations sur le jeu de réplicas, voir Ensembles de [réplicas de concepts.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
