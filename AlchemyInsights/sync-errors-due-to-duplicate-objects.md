---
title: 902 (erreurs de synchronisation dues à des objets en double)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781260"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Erreurs de synchronisation dues à des objets dupliqués

L'un des messages d'erreur suivants peut s'afficher à la fin de la synchronisation d'annuaires:
  
- Impossible de mettre à jour cet objet dans Microsoft Online Services, car les attributs suivants associés à cet objet ont des valeurs qui peuvent être déjà associées à un autre objet dans votre répertoire local.
    
- Un objet synchronisé avec la même adresse proxy existe déjà dans votre répertoire Microsoft Online Services.
    
- Impossible de mettre à jour cet objet car les attributs suivants associés à cet objet ont des valeurs qui peuvent déjà être associées à un autre objet dans vos services d'annuaire local: UserPrincipalName.
    
Pour identifier et résoudre le problème, téléchargez et exécutez l' [outil de correction d'erreur DirSync IdFix](https://www.microsoft.com/download/details.aspx?id=36832).
  
Pour plus d'informations, consultez la rubrique [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

