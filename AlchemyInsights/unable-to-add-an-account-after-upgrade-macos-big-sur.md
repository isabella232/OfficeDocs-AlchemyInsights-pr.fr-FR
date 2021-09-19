---
title: Impossible d’ajouter un compte après la mise à niveau vers macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446728"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Impossible d’ajouter un compte après la mise à niveau vers macOS 11.6 Big Sur

Après la mise à niveau vers macOS 11.6, votre compte OneDrive professionnel ou scolaire ou votre compte personnel OneDrive n’apparaît peut-être pas dans votre liste de comptes, et vous ne pourrez peut-être pas vous connecter à un deuxième compte à partir de l’application.

Il s’agit d’un problème nouveau relatif à la mise à niveau de macOS 11.6. Tant que le problème n’est pas résolu, vous pouvez accéder à vos contenus OneDrive à partir du web ou de votre appareil mobile. Microsoft travaille avec Apple pour restaurer les fonctionnalités de OneDrive.

Vous pouvez également lancer manuellement l’instance de OneDrive manquante à l’aide de Terminal. 

**Remarque** : cette solution de contournement fonctionne uniquement jusqu’à ce que OneDrive soit redémarré (par un redémarrage de l’ordinateur ou par une mise à jour de l’application OneDrive).

Si l’instance manquante est le compte personnel, ouvrez le Terminal et entrez :

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Si l’instance manquante est le compte professionnel ou scolaire, ouvrez le Terminal et entrez :

`open "/Applications/OneDrive.app" --new --args /client=Business1`

