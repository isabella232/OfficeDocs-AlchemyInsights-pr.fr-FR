---
title: Micro-retards ou limitations dans Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947831"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-retards ou limitations dans Exchange Online PowerShell

Vous pouvez remarquer des avertissements ou des retards de type « Micro-retard appliqué » lorsque vous exécutez des scripts et des applets de commande dans Exchange Online. Voici deux suggestions relatives à ce problème :

- Vous voudrez peut-être essayer d’utiliser le [module Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), qui inclut des applets de commande reposant sur l’API REST et qui sont considérablement plus performantes. Il peut s’agir de la solution idéale pour un grand nombre de d’applets de commande Get fréquemment utilisées.
- Si vous avez besoin d’utiliser des applets de commande qui ne sont pas encore couvertes dans le module v2, veuillez consulter [Exécution d’applets de commande PowerShell pour un grand nombre d’utilisateurs dans Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), qui évoque la façon de contourner des limitations attendues de PowerShell dans Exchange Online.
