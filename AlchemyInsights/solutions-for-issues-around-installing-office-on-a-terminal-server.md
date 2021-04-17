---
title: Solutions aux problèmes d'installation d'office sur un serveur Terminal Server
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
ms.openlocfilehash: 447fee84edc65861dc04038cfe6424249e94f843
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823605"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Solutions aux problèmes d'installation d'office sur un serveur Terminal Server

Pour utiliser l'activation d'ordinateurs partagés, vous devez avoir un abonnement qui inclut Microsoft 365 Apps for enterprise.
  
- Vérifier que l'activation d'ordinateurs partagés est activée
- Vérifier que l'activation a réussi
- Passer en revue les messages d'erreur pour l'activation d'ordinateurs partagés :
- « Les produits que nous avons trouvés dans votre compte ne peuvent pas être utilisés pour activer Office dans des scénarios d'ordinateur partagé »
  
Cette erreur signifie que vous n'avez pas d'abonnement qui inclut Microsoft 365 Apps for enterprise.

« Produit sans permis »

- Vérifiez que l'utilisateur se voit attribuer une licence pour Microsoft 365 Apps for enterprise.
- Vérifiez que l'utilisateur se signe avec son compte d'utilisateur.
- Vérifiez qu’il existe une connectivité entre l’ordinateur partagé et Internet.

Pour d'autres conseils de dépannage, voir : Résoudre les problèmes [d'activation d'ordinateurs partagés](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)