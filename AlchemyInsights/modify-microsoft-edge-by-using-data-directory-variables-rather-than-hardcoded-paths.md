---
title: Modifier les Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés en dur
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
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113414"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Modifier les Microsoft Edge à l’aide de variables de répertoire de données plutôt que de chemins d’accès codés en dur

Par exemple, sous Windows, pour stocker les données de profil sous les données d’application locales d’un utilisateur plutôt que dans l’emplacement par défaut, définissez la stratégie **UserDataDir** sur **${local_app_data}\Edge\Profile**. 

Pour plus d’informations, voir Créer Microsoft Edge variables du [répertoire de données utilisateur.](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)