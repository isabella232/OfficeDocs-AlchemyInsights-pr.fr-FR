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
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394687"
---
# <a name="sendas-mail-enabled-public-folder"></a>Dossier public envoyer en tant que courrier électronique

L’exemple suivant affecte des autorisations « Envoyer en tant que » pour le dossier public à extension messagerie NewPF1 à l’utilisateur Jason.

Add-RecipientPermission-Identity’NewPF1 '-Trustee "Jason"-AccessRights’SendAs'

Pour obtenir des informations détaillées sur la syntaxe et les paramètres, consultez la rubrique [attribuer des autorisations « Envoyer en tant que » ou « envoyer de la part de » pour les dossiers publics à extension messagerie](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).
