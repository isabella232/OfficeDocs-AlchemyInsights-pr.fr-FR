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
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103550"
---
# <a name="block-user-made-email-signatures"></a>Bloquer les signatures électroniques de l’utilisateur

La solution suivante s’applique uniquement aux signatures électroniques créées dans Outlook sur le web. Vous ne pouvez bloquer les signatures dans l’application Outlook que si vous avez une application Exchange Server.

1. Dans le Centre d’administration, **sélectionnez Centres**  >  **d’administration Exchange**.
2. Cliquez **sur autorisations**  >  **Outlook stratégies Web App.**
3. Sélectionnez la stratégie, puis cliquez sur l’icône de crayon pour la modifier.
4. Cliquez sur  >  **fonctionnalités Plus d’options**.
5. Sous **Expérience utilisateur,** cochez la case **Signature** électronique, puis cliquez sur **Enregistrer.**

**Important :** Si une signature a été ajoutée avant d’effacer cette case à cocher, l’utilisateur pourra toujours l’utiliser. Demandez-leur de le supprimer.
