---
title: 1554 erreur Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698860"
---
# <a name="winsock-error-10061"></a>Erreur Winsock 10061

Ce code d’erreur signifie que Microsoft n’a pas pu établir un socket TCP (connexion) avec l’hôte cible. La cause la plus probable de cette erreur est un problème avec la configuration de votre pare-feu. Pour résoudre le problème, vérifiez les paramètres suivants :

- Vérifier la configuration de votre pare-feu avec les informations contenues dans les [URL et plages d’adresses IP de Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Si l’erreur est spécifique à Exchange Online Protection (EOP), vous devriez avoir été préalablement notifié à une modification apportée aux [adresses IP d’Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Vérifiez que votre fournisseur de services Internet (ISP) ne bloque pas le port.

- Vérifiez les paramètres de l’hôte actif et du serveur cible dans vos connecteurs.

Notez que Microsoft 365 ne bloque pas les connexions *entrantes* de cette manière.
