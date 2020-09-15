---
title: Désactivation des groupes externes
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
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704126"
---
# <a name="how-to-disable-external-groups"></a>Désactivation des groupes externes

La messagerie externe Yammer applique les règles de transport Exchange (ETR), un ensemble de contrôles proactifs pour empêcher le partage des informations de l’entreprise. Pour empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer de façon à ce qu’il utilise la règle de transport Exchange pour bloquer la messagerie externe.
  
Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer :
  
- Connectez-vous à yammer en tant qu’administrateur vérifié, puis, dans le **Centre d’administration Yammer**, accédez à C **contenu and Security \> Security Settings.**

- Sous **messagerie externe**, sélectionnez **appliquer vos règles de transport Exchange Online Exchange (ETR) dans Yammer.**

- Cliquez sur **Enregistrer**.

Pour plus d’informations, consultez [la rubrique désactiver la messagerie externe dans un réseau Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  