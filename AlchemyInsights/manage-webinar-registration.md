---
title: Gérer l’inscription au webinaire
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783139"
---
# <a name="manage-webinar-registration"></a>Gérer l’inscription au webinaire

Vous pouvez gérer qui peut s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell. Pour installer Teams PowerShell, consultez [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Par défaut, *WhoCanRegister* est activé et défini sur **EveryoneInCompany**. Pour permettre à tout le monde, y compris aux utilisateurs anonymes, de s’inscrire, vous devez définir la stratégie de réunion sur **Tout le monde** à l’aide de la commande PowerShell :

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Remarque**: si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires. Pour en savoir plus et activer ce paramètre, consultez [Gérer les paramètres de réunion dans Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.

Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).
