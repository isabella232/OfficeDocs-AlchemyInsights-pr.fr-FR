---
title: Erreur 1554 Winsock 10061
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
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083228"
---
# <a name="winsock-error-10061"></a>Erreur Winsock 10061

Ce code d’erreur signifie que Microsoft n’a pas pu établir de socket TCP (connexion) avec l’hôte cible. La cause la plus probable de cette erreur est un problème avec la configuration de votre pare-feu. Pour résoudre le problème, vérifiez les paramètres ci-après :

- Vérifier la configuration de votre pare-feu avec les informations Microsoft 365 [URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Si l’erreur est spécifique à Exchange Online Protection (EOP), vous devez avoir été averti précédemment d’une modification des [adresses IP Exchange Online Protection’adresses IP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Vérifiez que votre fournisseur de services Internet (ISP) ne bloque pas le port.

- Vérifiez les paramètres de l’hôte intelligent et du serveur cible dans vos connecteurs.

Notez que Microsoft 365 ne bloque pas les *connexions* entrantes de cette manière.
