---
title: Microsoft teams-accès invité
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
ms.openlocfilehash: da9ecca062bd5f1dcc169657483ba53eb201def0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798374"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft teams-accès invité

Si vous avez besoin d’aide pour communiquer avec des utilisateurs extérieurs à votre organisation dans Teams, vous devez décider s’il faut utiliser [l’accès à des invités ou l’accès externe (Fédération)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)ou vous pouvez utiliser les deux.

Veillez à [passer en revue les différences](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) afin de comprendre les fonctionnalités disponibles pour chacune d’elles.  Par exemple, l’accès externe (Fédération) autorise des communications 1:1, comme la conversation et la présence.  Toutefois, les utilisateurs fédérés ne peuvent pas participer à la collaboration avec Teams.  Si vous souhaitez qu’un utilisateur externe rejoigne et participe à des conversations de canal teams ou partage des fichiers, vous devez activer l’accès invité.

**Option 1 : activer l’accès invité**   
Dans le centre d’administration Teams, accédez à paramètres d’organisation de l' [organisation > accès invité](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) et activez la fonction autoriser l’accès invité dans Teams.  Pour un client avec tous les autres paramètres par défaut, il vous suffit de le faire.  Pour personnaliser la configuration de l’accès invité, vérifiez que vous suivez toutes les étapes de la [liste de vérification d’accès invité](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Une fois que vous avez terminé, vous devrez [patienter jusqu’à 24 heures](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) pour que les paramètres prennent effet.

Si vous êtes certain d’avoir effectué toutes les étapes de la liste de vérification et qu’il y a plus de 24 heures, continuez et essayez d' [Ajouter un invité à votre équipe](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Pour plus d’informations, y compris des procédures, consultez la rubrique [accès invité dans Microsoft teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Option 2 : activer l’accès externe (Fédération)** Si vous souhaitez également activer l’accès externe (Fédération), dans le centre d’administration Teams, accédez à paramètres à l’échelle de l' [organisation > accès externe](https://admin.teams.microsoft.com/company-wide-settings/external-communications) et activez la « les utilisateurs peuvent communiquer avec les utilisateurs de Skype entreprise et de teams », puis suivez toutes les étapes de la rubrique [permettre à vos équipes de discuter et de communiquer avec les utilisateurs d’une autre organisation](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).


