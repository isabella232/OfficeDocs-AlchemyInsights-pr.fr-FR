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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760831"
---
# <a name="manage-webinar-registration"></a>Gérer l’inscription au webinaire

Vous pouvez gérer qui peut s’inscrire aux webinaires Teams à l’aide des commandes Teams PowerShell. Par défaut,  WhoCanRegister est activé et défini sur **Tout le monde**. Si vous souhaitez désactiver l’inscription à la réunion, définissez *AllowMeetingRegistration* sur **False**.

Pour modifier ces paramètres, vous devez installer [Teams PowerShell](/microsoftteams/teams-powershell-install). En outre, les stratégies de réunion sont appliquées aux webinaires Teams. Par exemple, si la participation anonyme est désactivée dans les paramètres de réunion, les utilisateurs anonymes ne peuvent pas participer aux webinaires.

Pour en savoir plus sur la configuration de qui peut s’inscrire aux webinaires, consultez [Configurer qui peut s’inscrire aux webinaires](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Pour plus d’informations sur les paramètres des listes Microsoft, consultez [Paramètres de contrôle pour Listes Microsoft](/sharepoint/control-lists).