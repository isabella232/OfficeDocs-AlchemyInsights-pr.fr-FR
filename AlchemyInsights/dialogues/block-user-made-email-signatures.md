---
title: Bloquer les signatures électroniques de l’utilisateur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232749"
---
# <a name="block-user-made-email-signatures"></a>Bloquer les signatures électroniques de l’utilisateur

La solution suivante s’applique uniquement aux signatures électroniques créées dans Outlook sur le web. Vous ne pouvez bloquer les signatures dans l’application Outlook que si vous avez une base de Exchange Server.

1. Dans le Centre d’administration, sélectionnez **Centres d’administration**  >  **Exchange**.
2. Cliquez sur **autorisations**  >  **Stratégies Outlook Web App.**
3. Sélectionnez la stratégie, puis cliquez sur l’icône de crayon pour la modifier.
4. Cliquez sur  >  **fonctionnalités Plus d’options**.
5. Sous **Expérience utilisateur,** cochez la case **Signature** électronique, puis cliquez sur **Enregistrer.**

**Important :** Si une signature a été ajoutée avant d’effacer cette case à cocher, l’utilisateur pourra toujours l’utiliser. Demandez-leur de le supprimer.
