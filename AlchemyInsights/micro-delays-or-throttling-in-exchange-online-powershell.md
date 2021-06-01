---
title: Micro-retards ou limitations dans Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702124"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro-retards ou limitations dans Exchange Online PowerShell

Vous pouvez remarquer des avertissements ou des retards de type « Micro-retard appliqué » lorsque vous exécutez des scripts et des applets de commande dans Exchange Online. Voici quelques suggestions pour résoudre ce problème :

- Veuillez exécuter nos diagnostics pour assouplir les stratégies PowerShell de limitation de votre client. Cette solution corrige le problème pour la majorité.
- Si le problème persiste, utilisez le [module Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), qui inclut des applets de commande reposant sur l’API REST et qui sont considérablement plus performantes. Il peut s’agir de la solution idéale pour un grand nombre de d’applets de commande Get- fréquemment utilisées.
- Si vous avez besoin d’utiliser des applets de commande qui ne sont pas couvertes dans le module v2, veuillez consulter [Exécution d’applets de commande PowerShell pour un grand nombre d’utilisateurs dans Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), qui évoque la façon de contourner des limitations de PowerShell dans Exchange Online.
