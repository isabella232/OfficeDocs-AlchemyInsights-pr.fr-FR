---
title: Empêcher le déplacement automatique des messages vers l’archive
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522391"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>Empêcher le déplacement automatique des messages vers l’archive

Si vous utilisez une stratégie de rétention, vous pouvez modifier l’âge de rétention dans cette stratégie pour arrêter automatiquement l’archivage des messages. Voici comment procéder :

1. Dans le Centre [d’administration Exchange,](https://go.microsoft.com/fwlink/?linkid=2059104)choisissez les **balises de rétention de gestion** de la  >  **conformité.** Recherchez votre balise de rétention Déplacer vers l’archive.
2. Dans la balise de rétention, modifiez  la période de rétention (période d’archivage) pour ne jamais empêcher les éléments d’être automatiquement archivés par une stratégie de rétention.

> [!NOTE]
> Cela modifie le paramètre d’archivage de toutes les boîtes aux lettres avec cette balise de rétention qui leur est appliquée.
