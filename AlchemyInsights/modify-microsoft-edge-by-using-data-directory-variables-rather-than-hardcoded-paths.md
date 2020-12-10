---
title: Modifier Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608843"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modifier Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés

Par exemple, sous Windows, pour stocker les données de profil sous les données d’application locale d’un utilisateur plutôt que dans l’emplacement par défaut, définissez la stratégie **UserDataDir** sur **$ {local_app_data} \Edge\Profile**. 

Pour plus d’informations, consultez la rubrique [Create Microsoft Edge User Data Directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).