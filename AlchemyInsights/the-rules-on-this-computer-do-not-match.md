---
title: 'Erreur : les règles de cet ordinateur ne correspondent pas.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617969"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Erreur : les règles de cet ordinateur ne correspondent pas.

Pour afficher l’État mis à jour de ce problème connu, consultez [les règles de cet ordinateur ne correspondent pas aux règles de Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

L’équipe Outlook a implémenté un correctif dans Build 12928,10000. Le correctif est déjà Insider rapidement et sera dirigé vers le canal mensuel de la fin du 2020 juin. Une fois que vous disposez de la version corrigée, vous pouvez obtenir l’invite « quelles règles souhaitez-vous conserver » une dernière fois. Choisissez serveur lorsque vous y êtes invité, puis revenez dans Outlook et réactivez toutes les règles qui ont été désactivées.

Tant que le correctif n’est pas disponible, utilisez la solution de contournement suivante :

**Solution**: dans les rapports récents, le problème s’est produit pour ceux qui ont uniquement créé des règles de client dans le bureau Outlook. Si vous continuez à rencontrer le problème, envisagez de supprimer les règles, puis créez et modifiez des règles uniquement dans OWA (Outlook Web App) jusqu’à ce que le problème soit résolu.

Si vous ne pouvez pas supprimer les règles manuellement, vous pouvez exécuter une commande Outlook lorsque vous démarrez Outlook en exécutant Outlook. exe/Cleanrules. Cette opération supprimera les règles client et serveur. Il supprime toutes les règles de tous les comptes dans le profil Outlook. Cette commande est encore documentée dans l’article des commutateurs de ligne de commande.