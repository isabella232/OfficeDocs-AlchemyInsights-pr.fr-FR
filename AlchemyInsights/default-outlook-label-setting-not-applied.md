---
title: Paramètre d’Outlook par défaut non appliqué
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58370210"
---
# <a name="default-outlook-label-setting-not-applied"></a>Paramètre d’Outlook par défaut non appliqué

Si vos paramètres d’étiquette par défaut Outlook ne s’appliquent pas correctement et qu’une autre étiquette ou aucune étiquette n’est appliquée, vous pouvez être confronté à un problème connu (MC277818) et faire l’une de ces deux options pour résoudre le problème :

**Option 1 :**

1. Go to Microsoft 365 Compliance Center > **Solutions**  >  **Information Protection**.
1. Sélectionnez **les** stratégies d’étiquette, puis sélectionnez la stratégie d’étiquette que vous devez modifier ( le **paramètre OutlookDefaultlabel** n’est pas correctement définie sur la stratégie d’étiquette en question. Exécutez **Get-labelpolicy pour** afficher ce paramètre), puis sélectionnez **Modifier la stratégie.**
1. **Sélectionnez** Suivant jusqu’à ce que le paramètre Appliquer cette étiquette par défaut aux e-mails **,** qui est disponible si vous sélectionnez Exiger que les utilisateurs appliquent une étiquette pour obliger les e-mails et **les documents** dans la boîte de dialogue **Paramètres** de stratégie.
1. Dans la **boîte de dialogue Appliquer une étiquette par défaut aux documents,** choisissez **Aucune** dans la liste liste.
1. Sélectionnez **Suivant** **et Envoyer** pour enregistrer vos paramètres d’étiquette.

**Option 2 :**

Dans le Centre de sécurité et conformité [Powershell,](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)utilisez l'Set-LabelPolicy commandlet pour modifier La valeur **OutlookDefaultlabel** sur **Aucun** sur {OutlookDefaultLabel="None"}.

Exécutez : `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Pour plus d’informations sur les étiquettes par Outlook, voir Définir une autre étiquette par défaut [pour Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).