---
title: 902 (erreurs de synchronisation dues à des objets en double)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737339"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erreurs de synchronisation dues à des objets dupliqués

Vous pouvez recevoir l’un des messages d’erreur suivants lorsque la synchronisation d’annuaires se termine dans Microsoft 365 :

- Impossible de mettre à jour cet objet dans Microsoft Online Services, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associées à un autre objet dans votre répertoire local.

- Un objet synchronisé avec la même adresse proxy existe déjà dans votre répertoire Microsoft Online Services.

- Impossible de mettre à jour cet objet car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans vos services d’annuaire local : UserPrincipalName.

Pour identifier et résoudre le problème, téléchargez et exécutez l' [outil de correction d’erreur DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).

Pour plus d’informations, consultez la rubrique [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
