---
title: Libérer de l’espace disque dans Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928079"
---
# <a name="free-up-drive-space-in-windows-10"></a>Libérer de l’espace disque dans Windows 10

Deux options s’offrent à vous pour libérer de l’espace sur le lecteur dans Windows :

- Libérer de l’espace disque dans Windows 10.
- Libérez de l’espace pour les mises à jour Windows 10 avec un périphérique de stockage externe.

Si vous disposez toujours d'un faible espace disque après avoir utilisé le nettoyage de disque, il est possible que votre dossier Temp se remplisse rapidement de fichiers d'application (.appx) utilisés par Microsoft Store. Pour résoudre ce problème, réinitialisez le Store, effacez le cache du Store, puis exécutez l'outil de résolution des problèmes de Windows Update. Avant de procéder, assurez-vous que Microsoft Store est fermé.

**Étape 1 : réinitialiser Microsoft Store**

**Remarque** cette application supprime définitivement les données de l’application sur l’appareil, y compris vos préférences et les détails de la connectez-vous.

1. Sélectionnez **Démarrer** > **Paramètres** > **Applications** > **Applications et fonctionnalités**.

1. Dans la liste des applications, recherchez et sélectionnez Microsoft Store.

1. Sélectionnez **Options avancées**.

1. Faites défiler vers le bas et sélectionnez **Réinitialiser**, puis **Confirmer la réinitialisation**.

**Étape 2 : effacer le cache du Microsoft Store**

1. Appuyez sur la touche de logo Windows+R pour ouvrir la boîte de dialogue Exécuter.

1. Tapez wsreset.exe, puis sélectionnez **OK**.

1. Une fenêtre d’invite de commandes vide s’ouvre. Après environ 10 secondes, la fenêtre se ferme et le Store s’ouvre automatiquement.

**Étape 3 : réinitialiser Windows Update**

1. Sélectionnez **Démarrer** > **Paramètres** > **Mise à jour et sécurité,** > **Résoudre des problèmes**.

1. Faites défiler vers le bas et sélectionnez **Windows Update** dans la liste, puis sélectionnez **Exécuter l’utilitaire de résolution des problèmes**.

1. Redémarrez votre ordinateur et vérifiez que vous rencontrez toujours le problème.

