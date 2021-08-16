---
title: Solutions aux problèmes d’installation d’office sur un serveur Terminal Server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 28ebe2b1375b142ca63dc686c7afbbe88abfd539a93780cff3861f80de40b411
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021846"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Solutions aux problèmes d’installation d’office sur un serveur Terminal Server

Pour utiliser l’activation d’ordinateurs partagés, vous devez avoir un abonnement qui inclut Applications Microsoft 365 pour les grandes entreprises.
  
- Vérifier que l’activation d’ordinateurs partagés est activée
- Vérifier que l’activation a réussi
- Passer en revue les messages d’erreur pour l’activation d’ordinateurs partagés :
- « Les produits que nous avons trouvés dans votre compte ne peuvent pas être utilisés pour activer des Office dans des scénarios d’ordinateurs partagés »
  
Cette erreur signifie que vous n’avez pas d’abonnement incluant Applications Microsoft 365 pour les grandes entreprises.

« Produit sans permis »

- Vérifiez que l’utilisateur se voit attribuer une licence pour Applications Microsoft 365 pour les grandes entreprises.
- Vérifiez que l’utilisateur se signe avec son compte d’utilisateur.
- Vérifiez qu’il existe une connectivité entre l’ordinateur partagé et Internet.

Pour d’autres conseils de dépannage, voir : Résoudre les problèmes [d’activation d’ordinateurs partagés](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)