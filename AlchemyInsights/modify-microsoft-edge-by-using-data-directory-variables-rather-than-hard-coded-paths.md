---
title: Modifier Microsoft Edge à l’aide de variables du répertoire de données plutôt que de chemins d’accès codés en dur
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897625"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Modifier Microsoft Edge à l’aide de variables du répertoire de données plutôt que de chemins d’accès codés en dur

Par exemple, sous Windows, pour stocker les données de profil sous les données d’application locales d’un utilisateur plutôt que dans l’emplacement par défaut, définissez la stratégie *UserDataDir* sur **${local_app_data}\Edge\Profile**.

Pour plus d’informations, consultez [Créer des variables de répertoire de données utilisateur Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).