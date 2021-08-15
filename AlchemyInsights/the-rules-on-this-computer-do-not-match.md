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
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981111"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erreur : les règles sur cet ordinateur ne correspondent pas

Pour voir l’état mis à jour de ce problème [connu,](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) consultez Les règles de cet ordinateur ne correspondent pas aux règles sur Microsoft Exchange

L Outlook a implémenté un correctif dans la build 12928.10000. The fix is already at Insider Fast and will go to Monthly Channel in late June 2020. Une fois que vous avez la build fixe, vous pouvez obtenir l’invite « Quelles règles voulez-vous conserver » une dernière fois. Choisissez Serveur lorsque vous y êtes invité, puis revenir dans Outlook puis réactivez les règles qui ont été désactivées.

Jusqu’à ce que le correctif soit disponible, utilisez la solution de contournement suivante :

**Solution de contournement**: dans les rapports récents, le problème s’est produit pour ceux qui ont uniquement créé des règles client dans Outlook bureau. Si vous continuez à vous lancer dans le problème, envisagez de supprimer les règles, puis créez et modifiez des règles uniquement dans OWA (Outlook Web App) jusqu’à ce que le problème soit résolu.

Si vous ne pouvez pas supprimer les règles manuellement, vous pouvez exécuter une commande Outlook lorsque vous démarrez Outlook en exécutant Outlook.exe /cleanrules. Cela supprime à la fois les règles client et serveur. Elle supprime toutes les règles de tous les comptes du profil Outlook client. Cette commande est davantage documentée dans l’article Commutateurs de ligne de commande.

