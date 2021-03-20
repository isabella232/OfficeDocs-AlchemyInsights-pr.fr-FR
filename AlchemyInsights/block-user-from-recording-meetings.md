---
title: Empêcher l’utilisateur d’enregistrer des réunions
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
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897674"
---
# <a name="block-user-from-recording-meetings"></a>Empêcher l’utilisateur d’enregistrer des réunions

Si vous devez empêcher ou **empêcher** des utilisateurs spécifiques d’enregistrer des réunions Teams, vous pouvez le faire via les paramètres de stratégie de réunion Teams. Dans le Centre d’administration Microsoft Teams, désactiver le paramètre Autoriser l’enregistrement **dans le cloud** dans la stratégie de réunion attribuée à cet utilisateur. Pour plus d’informations, voir [Gérer les stratégies de réunion dans Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

Pour vérifier si un utilisateur spécifique est autorisé ou non à enregistrer des réunions Teams, utilisez le diagnostic de support. Exécutez une nouvelle requête de support et tapez **diag : enregistrement** de réunion : le diagnostic vérifie les paramètres de stratégie pour l’utilisateur spécifié et détermine ses paramètres de stratégie. N’oubliez pas que l’application des nouveaux paramètres de stratégie peut prendre quelques heures. Par exemple, si vous avez apporté une modification, patientez quelques heures avant de recommencer le diagnostic.

Pour plus d’informations, [examinez Activer ou désactiver l’enregistrement dans le cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
