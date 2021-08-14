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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998792"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erreurs de synchronisation dues à des objets en double

Vous pouvez recevoir l’un des messages d’erreur suivants lorsque la synchronisation d’annuaires se termine Microsoft 365 :

- Impossible de mettre à jour cet objet dans Microsoft Online Services car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans votre répertoire local.

- Un objet synchronisé avec la même adresse proxy existe déjà dans Microsoft Online Services répertoire.

- Impossible de mettre à jour cet objet car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans vos services d’annuaire local : UserPrincipalName.

Pour identifier et résoudre le problème, téléchargez et exécutez l’outil de correction des [erreurs DirSync IdFix.](https://github.com/Microsoft/idfix)

Pour plus d’informations, [voir KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
