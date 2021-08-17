---
title: Dossier public à messagerie envoyer en tant que dans EXO
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
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052564"
---
# <a name="sendas-mail-enabled-public-folder"></a>Dossier public à messagerie SendAs

L’exemple suivant attribue des autorisations « Envoyer en tant que » pour le dossier public à messagerie NewPF1 à l’utilisateur Quinte.

Add-RecipientPermission -Identity 'NewPF1' -Trustee « Cée » -AccessRights 'SendAs'

Pour obtenir des informations détaillées sur la syntaxe et les [paramètres,](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)voir Attribuer des autorisations « Envoyer en tant que » ou « Envoyer de la part de » pour les dossiers publics à messagerie.

