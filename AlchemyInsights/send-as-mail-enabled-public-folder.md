---
title: Envoyer en tant que dossier public à extension messagerie dans EXO
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
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451381"
---
# <a name="sendas-mail-enabled-public-folder"></a>Dossier public envoyer en tant que courrier électronique

L’exemple suivant affecte des autorisations « Envoyer en tant que » pour le dossier public à extension messagerie NewPF1 à l’utilisateur Jason.

Add-RecipientPermission-Identity’NewPF1 '-Trustee "Jason"-AccessRights’SendAs'

Pour obtenir des informations détaillées sur la syntaxe et les paramètres, consultez la rubrique [attribuer des autorisations « Envoyer en tant que » ou « envoyer de la part de » pour les dossiers publics à extension messagerie](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).

