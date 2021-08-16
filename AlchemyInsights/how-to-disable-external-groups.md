---
title: Comment désactiver les groupes externes
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015618"
---
# <a name="how-to-disable-external-groups"></a>Comment désactiver les groupes externes

Yammer messagerie externe s’applique Exchange règles de transport (ETR), un ensemble de contrôles proactifs pour empêcher le partage des informations de l’entreprise. Pour empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer pour utiliser la règle de transport Exchange afin de bloquer la messagerie externe.
  
Une fois que vous avez créé une règle dans Exchange Online centre d’administration, suivez les étapes suivantes pour définir ETR à appliquer dans Yammer :
  
- Connectez-vous Yammer en tant qu’administrateur vérifié et, dans le centre **d’administration Yammer,** allez à C **Content and Security \> Paramètres.**

- Sous **Messagerie externe,** sélectionnez Appliquer vos règles Exchange Online Exchange transport de messagerie électronique **(ETR) dans Yammer.**

- Cliquez sur **Enregistrer**.

Pour plus d’informations, voir [Désactiver la messagerie externe dans un Yammer réseau.](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)
  