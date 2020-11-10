---
title: Utilisation de images giphy dans les conversations de teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947491"
---
# <a name="using-giphys-in-teams-conversations"></a>Utilisation de images giphy dans les conversations de teams

L’accès images giphy dans Team Chat est activé par défaut. En tant qu’administrateur, vous pouvez contrôler si images giphy est disponible pour les utilisateurs en [définissant une stratégie de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) et en vous assurant que **l’utilisation de images giphy dans les conversations** est **activée**.

Si les images gif ne fonctionnent pas comme prévu dans les conversations de teams, vérifiez les éléments suivants :

La [stratégie de messagerie](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) doit autoriser images giphy. Pour vérifier à l’aide des cmdlets PowerShell, procédez comme suit :

- Vérifiez que vous pouvez [gérer teams avec PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Exécutez la commande PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) et vérifiez que **AllowGiphy** est défini sur **true**.
- Si **AllowGiphy** est défini sur **false** , exécutez la commande PowerShell suivante [Set-CsTeamsMessagingPolicy-identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Les [expériences en connexion facultatives](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) doivent être activées pour permettre l’accès à l’URL Giphy.

> [!NOTE]
> Si plusieurs stratégies de messagerie de teams sont configurées pour votre client, vous pouvez déterminer l’identité de la stratégie attribuée à l’utilisateur concerné à l’aide de la commande PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Sélectionnez TeamsMessagingPolicy.
