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
ms.openlocfilehash: df7443626308416e1d7edf4bc87c0eba95ec2c030d5ef3207513480873c1e3e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929951"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>Empêcher le déplacement automatique des messages vers l’archive

Si vous utilisez une stratégie de rétention, vous pouvez modifier l’âge de rétention dans cette stratégie pour arrêter automatiquement l’archivage des messages. Voici comment procéder :

1. Dans le centre [Exchange' administration,](https://go.microsoft.com/fwlink/?linkid=2059104)choisissez les **balises** de rétention de gestion  >  **de la conformité.** Recherchez votre balise de rétention Déplacer vers l’archive.
2. Dans la balise de rétention, modifiez  la période de rétention (période d’archivage) pour ne jamais empêcher les éléments d’être automatiquement archivés par une stratégie de rétention.

> [!NOTE]
> Cela modifie le paramètre d’archivage de toutes les boîtes aux lettres avec cette balise de rétention qui leur est appliquée.
