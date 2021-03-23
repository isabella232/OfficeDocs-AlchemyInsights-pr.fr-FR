---
title: À propos Yammer administrateurs
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995260"
---
# <a name="about-yammer-admins"></a>À propos Yammer administrateurs

**Administrateurs réseau**

Les administrateurs globaux sont automatiquement promus au rôle d’administrateur vérifié dans Yammer réseau. Dans les cas suivants, cette promotion peut ne pas se produire correctement :

- Plusieurs Yammer réseaux existants, et l’administrateur est en train d’être en train d’être en communication avec le mauvais réseau. [La consolidation du](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) réseau est nécessaire pour obtenir un Yammer réseau.
- Azure PIM est en cours d’utilisation. L’utilisateur peut ne pas être promu en tant qu’administrateur global suffisamment longtemps pour que la promotion se produise. Une prochaine mise à jour Yammer peut résoudre ce problème, mais il est préférable de promouvoir manuellement les utilisateurs en tant qu’administrateurs globaux.
- Il existe un problème de synchronisation avec Yammer réseau. Dans ce cas, une demande de support sera requise pour une investigation plus approfondie.

Pour plus d’informations sur Yammer rôles d’administrateur, voir [Gérer Yammer administrateurs.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)

**Administrateurs de groupe**

Les administrateurs de groupe pour les groupes connectés à Microsoft 365 sont synchronisés avec l’appartenance à un groupe à partir d’Azure AD. Pour les grands groupes, cette synchronisation peut prendre une période prolongée.
