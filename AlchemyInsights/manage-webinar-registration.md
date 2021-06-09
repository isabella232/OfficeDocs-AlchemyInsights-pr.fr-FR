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
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798642"
---
# <a name="manage-webinar-registration"></a>Gérer l’inscription au webinaire

Vous pouvez gérer qui peut s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell. Pour installer Teams PowerShell, consultez [Teams PowerShell](/microsoftteams/teams-powershell-install). 

Par défaut, *WhoCanRegister* est activé et défini sur **Tout le monde**. 

Si vous ne voyez pas l’option permettant d’autoriser l’inscription à Tout le monde dans l’invitation à la réunion, réexécutez le paramètre *WhoCanRegister* à Tout le monde et attendez 24 heures. Pour réexécuter *WhoCanRegister*, utilisez la commande PowerShell :

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Remarque**: si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires. Pour en savoir plus et activer ce paramètre, consultez [Gérer les paramètres de réunion dans Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.

Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).
