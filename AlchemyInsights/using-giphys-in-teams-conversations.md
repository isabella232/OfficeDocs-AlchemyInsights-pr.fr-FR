---
title: Utilisation de Giphys dans Teams conversations
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323518"
---
# <a name="using-giphys-in-teams-conversations"></a>Utilisation de Giphys dans Teams conversations

L’accès giphys dans Teams conversation est activé par défaut. En tant qu’administrateur, vous pouvez contrôler si [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphys est disponible pour les utilisateurs en établissant une stratégie de messagerie et en vous assurant que l’utilisation de **Giphys** dans les conversations **est sur .**

Si les gif ne fonctionnent pas comme prévu dans Teams conversations, vérifiez :

La [stratégie de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) doit autoriser Giphys. Pour vérifier à l’aide des cmdlets PowerShell :

- Vérifiez que vous pouvez gérer [les Teams avec PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Exécutez la commande PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) et vérifiez que **AllowGiphy** est définie sur **TRUE**.
- Si **AllowGiphy est** définie sur **FALSE,** exécutez la commande PowerShell [suivante Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Les expériences connectées](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) facultatives doivent être activées pour autoriser l’accès à l’URL Giphy.

Remarque : si plusieurs stratégies de messagerie Teams sont configurées pour votre client, vous pouvez déterminer l’identité de la stratégie attribuée à l’utilisateur affecté avec la commande PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Sélectionnez TeamsMessagingPolicy.
