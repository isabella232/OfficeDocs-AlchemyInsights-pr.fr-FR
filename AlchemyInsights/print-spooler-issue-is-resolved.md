---
title: Le problème de spouleur d’impression est résolu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083948"
---
# <a name="print-spooler-issue-is-resolved"></a>Le problème de spouleur d’impression est résolu

Si votre appareil a été mis à jour avec Windows 10 **Système d’exploitation Build 19041.329**, vous avez peut-être remarqué un problème dans lequel certaines imprimantes n’ont pas pu être imprimées. Il se peut que le spouleur d’impression génère une erreur ou se ferme de manière inattendue lors de la tentative d’impression et qu’aucune sortie ne provient de l’imprimante affectée. Ce problème a été résolu dans la version dusystème d’exploitation **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Examen continu**

Le fichier LSASS (service de sous-système d’autorité de sécurité locale) (**isass.exe**) peut échouer sur certains appareils avec le message d’erreur « un processus système critique, C:\WINDOWS\system32\Isass.exe, a échoué avec le code d’État c0000008. L’ordinateur doit maintenant être redémarré ».  **Microsoft travaille sur une résolution et fournit une mise à jour dans une prochaine publication.**

Pour plus d’informations, consultez [problèmes connus Windows 10 version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).