---
title: 'Erreur : les règles sur cet ordinateur ne correspondent pas'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782950"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erreur : les règles sur cet ordinateur ne correspondent pas

Pour voir l'état mis à jour de ce problème connu, consultez Les règles de cet ordinateur ne correspondent pas aux règles [sur Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

L'équipe Outlook a implémenté un correctif dans la build 12928.10000. The fix is already at Insider Fast and will go to Monthly Channel in late June 2020. Une fois que vous avez la build fixe, vous pouvez obtenir l'invite « Quelles règles voulez-vous conserver » une dernière fois. Sélectionnez Serveur lorsque vous y êtes invité, puis revenir dans Outlook et réactivez les règles qui ont été désactivées.

Jusqu'à ce que le correctif soit disponible, utilisez la solution de contournement suivante :

**Solution de contournement**: dans les rapports récents, le problème s'est produit pour ceux qui ont uniquement créé des règles client dans le bureau Outlook. Si vous continuez à vous lancer dans le problème, envisagez de supprimer les règles, puis créez et modifiez des règles uniquement dans OWA (Outlook Web App) jusqu'à ce que le problème soit résolu.

Si vous ne pouvez pas supprimer les règles manuellement, vous pouvez exécuter une commande Outlook lorsque vous démarrez Outlook en exécutant Outlook.exe /cleanrules. Cela supprime à la fois les règles client et serveur. Il supprime toutes les règles pour tous les comptes du profil Outlook. Cette commande est davantage documentée dans l'article Commutateurs de ligne de commande.

