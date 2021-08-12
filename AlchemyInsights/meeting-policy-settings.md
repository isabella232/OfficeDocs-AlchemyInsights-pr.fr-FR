---
title: Paramètres de stratégie de réunion
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925163"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Gérer les stratégies de réunion dans Microsoft Teams

**Remarque : l’application des modifications de stratégie pour les utilisateurs peut prendre jusqu’à 24 heures.** Il se peut que vous ne soyez pas en mesure d’apporter immédiatement des modifications aux stratégies nouvellement créées ; patientez 4 heures et tentez à nouveau de modifier une stratégie nouvellement créée.

Stratégies de réunion: elles sont utilisées pour contrôler les fonctionnalités disponibles aux participants à la réunion pour les réunions planifiées par des utilisateurs au sein de votre organisation. Certaines fonctionnalités des stratégies de réunion peuvent ne pas encore être implémentées dans le Centre d’administration Teams (celles-ci sont étiquetées « bientôt » dans la documentation). Dans ce cas, ou si vous êtes en train d’obtenir une erreur telle que « Nous ne pouvons pas mettre à jour la stratégie pour le moment, mais essayer à nouveau plus tard » dans le Centre d’administration Microsoft Teams, nous vous recommandons d’utiliser PowerShell pour créer ou modifier des stratégies de réunion Teams. 

Pour plus d’informations sur les stratégies de réunion, consultez les ressources suivantes :

- Pour en savoir plus sur la création de stratégies, les modifications et l’affectation d’utilisateurs à la stratégie, voir Gérer les stratégies de réunion [dans Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Pour apporter des modifications de stratégie à l’aide des cmdlets PowerShell, [voir Teams vue d’ensemble de PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Vous devez utiliser le [module Skype Entreprise PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) pour Teams stratégies de réunion. 
    - Pour plus d’informations, veuillez consulter la documentation des [cmdlets *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

