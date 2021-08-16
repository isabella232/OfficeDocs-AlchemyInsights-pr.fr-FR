---
title: Microsoft Teams - Accès invité
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012306"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - Accès invité

Si vous avez besoin d’aide pour communiquer avec des utilisateurs extérieurs à votre organisation dans Teams, vous devez décider d’utiliser l’accès invité ou l’accès externe [(fédération)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)ou les deux.

N’oubliez [pas de passer en revue les différences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) pour comprendre les fonctionnalités disponibles pour chacune d’elles.  Par exemple, l’accès externe (fédération) autorise les communications 1:1, telles que la conversation et la présence.  Toutefois, les utilisateurs fédérés ne peuvent pas Teams collaboration.  Si vous souhaitez qu’un utilisateur externe rejoigne et participe à Teams conversations de canal ou partage de fichiers, vous devez activer l’accès invité.

**Option 1 : activer l’accès invité** Dans le Teams Admin Center, accédez à [l’Paramètres >](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) Invité à l’échelle de l’organisation et activer « Autoriser l’accès invité dans Teams ».  Pour un client avec tous les autres paramètres par défaut, il doit s’agit de tout ce que vous devez faire.  Pour personnaliser votre configuration d’accès invité, veillez à suivre toutes les étapes de la liste de contrôle [d’accès invité.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) Une fois que vous avez terminé, vous devrez patienter [jusqu’à 24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) heures pour que les paramètres prennent effet.

Si vous êtes sûr d’avoir effectué toutes les étapes de la liste de contrôle et que cela fait plus de 24 heures, essayez d’ajouter un invité à votre [équipe.](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)

Pour plus d’informations, y compris des vidéos de pratiques, voir [l’accès invité dans Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Option 2 : activer l’accès externe (fédération)** Si vous souhaitez également activer l’accès externe (Fédération), dans le Centre d’administration Teams accédez à [l’Paramètres >](https://admin.teams.microsoft.com/company-wide-settings/external-communications) Accès externe à l’échelle de l’organisation et activer « Les utilisateurs peuvent communiquer avec les utilisateurs Skype Entreprise et Teams », puis suivez toutes les étapes de la procédure de la page Laisser les utilisateurs de votre [Teams](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)discuter et communiquer avec des utilisateurs d’une autre organisation.
