---
title: Activer les webinaires Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: a56abdaae182b840a1a96466e0581ef49b2b0075
ms.sourcegitcommit: 540a4e2515f7cfddee65519046454fc4437cd287
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/01/2021
ms.locfileid: "53688972"
---
# <a name="enable-teams-webinars"></a>Activer les webinaires Teams

L'inscription au webinaire est activée par défaut. Si vous souhaitez désactiver l'inscription aux réunions, vous pouvez utiliser le centre d'administration Teams : 

1. Accédez au [Centre d’administration Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Sélectionnez la stratégie **globale (par défaut à l'échelle de l'organisation)** ou une autre stratégie spécifique. 

3. Sous **général**, définissez **Autoriser l’inscription aux réunions** sur **Désactivé**. 

Lorsque l'inscription à la réunion est définie sur **Activé**, vous pouvez également gérer les personnes qui s'inscrivent aux webinaires Teams à l'aide du centre d'administration Teams : 

1. Accédez au [Centre d’administration Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Sélectionnez la stratégie **globale (par défaut à l'échelle de l'organisation)** ou une autre stratégie spécifique. 

3. Sous **Général**, accédez au paramètre **Qui peut s’inscrire** et sélectionnez **Tout le monde** ou **Tout le monde dans l’entreprise**. 

**Remarque** : si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires. Pour en savoir plus et activer ce paramètre, consultez  [Gérer les paramètres de réunion dans Microsoft Teams](/microsoftteams/meeting-settings-in-teams). 

Pour en savoir plus sur la configuration des personnes autorisées à s’inscrire aux webinaires et sur la gestion de ces stratégies à l’aide de Teams PowerShell, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Pour plus d’informations sur les paramètres des listes Microsoft, consultez  [Paramètres de contrôle pour les Listes Microsoft](/sharepoint/control-lists). 