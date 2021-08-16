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
ms.openlocfilehash: 7eb3fd34ec6f1a2d431ed276b00dd46b5ec6aa73d69b37ef88b1ba0ca6f5d077
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019182"
---
# <a name="block-user-from-recording-meetings"></a>Empêcher l’utilisateur d’enregistrer des réunions

Si vous  devez empêcher ou empêcher des utilisateurs spécifiques d’enregistrer Teams réunions, vous pouvez le faire via les paramètres Teams stratégie de réunion. Dans le Microsoft Teams d’administration, désactiver le paramètre Autoriser l’enregistrement dans le **cloud** dans la stratégie de réunion attribuée à cet utilisateur. Pour plus d’informations, voir [Gérer les stratégies de réunion dans Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).

Pour vérifier si un utilisateur spécifique est autorisé ou non à enregistrer Teams réunions, utilisez le diagnostic de support. Exécutez une nouvelle requête de support et tapez **diag : enregistrement** de réunion : le diagnostic vérifie les paramètres de stratégie pour l’utilisateur spécifié et détermine ses paramètres de stratégie. N’oubliez pas que l’application des nouveaux paramètres de stratégie peut prendre quelques heures. Par exemple, si vous avez apporté une modification, patientez quelques heures avant de recommencer le diagnostic.

Pour plus d’informations, [examinez Activer ou désactiver l’enregistrement dans le cloud.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
