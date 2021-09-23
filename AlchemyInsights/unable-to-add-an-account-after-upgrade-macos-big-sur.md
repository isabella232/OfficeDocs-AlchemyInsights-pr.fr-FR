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
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475126"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Impossible d’ajouter un compte après la mise à niveau vers macOS 11.6 Big Sur

Après la mise à niveau vers macOS 11.6, votre compte OneDrive professionnel ou scolaire ou votre compte personnel OneDrive n’apparaît peut-être pas dans votre liste de comptes, et vous ne pourrez peut-être pas vous connecter à un deuxième compte à partir de l’application.

Un correctif a été développé pour ce problème. Tout d’abord, déterminez si vous exécutez la version autonome ou la version OneDrive de l’App Store :

- Sélectionnez le cloud OneDrive dans la barre de menus > **Aide et paramètres** > **Préférences** > **À propos de**. Si le numéro de version n’inclut pas **(Autonome)**, vous avez la version App Store du produit.

Si vous utilisez la version autonome de OneDrive, redémarrez votre ordinateur pour que OneDrive se mette automatiquement à jour vers une build dans laquelle ce problème est résolu. Si vous souhaitez installer la build manuellement, téléchargez ce [fichier .zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), décompressez le fichier, puis copiez l’application OneDrive dans le dossier Applications (en remplaçant l’application OneDrive existante).

Si vous utilisez la version de l’App Store, envisagez d’installer la version autonome de OneDrive. Cette version fonctionne de la même manière que la version de l’App Store, mais elle permet à Microsoft de proposer des mises à jour plus rapidement aux utilisateurs et de les connecter à une version qui inclut le correctif pour ce problème.

1. Téléchargez la version autonome de [OneDrive qui inclut le correctif.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Décompressez le fichier, puis copiez l’application OneDrive dans le dossier Applications (en remplaçant l’application OneDrive existante).

Si vous devez utiliser la version de l’App Store, attendez que l’App Store publie une version de l’application qui inclut le correctif. Malheureusement, Microsoft ne peut pas communiquer une date estimée pour la publication d’une version corrigée à partir de l’App Store.


