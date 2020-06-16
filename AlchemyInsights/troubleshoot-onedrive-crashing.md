---
title: Résoudre les problèmes liés à OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/15/2020
ms.locfileid: "44735389"
---
# <a name="troubleshoot-onedrive-crashes"></a>Résoudre les problèmes liés à OneDrive

Si OneDrive se bloque plusieurs fois, procédez comme suit pour résoudre les problèmes :

**Vérifiez que les clés du Registre ne sont pas fixées :**

1. À l’aide de l’Éditeur du Registre, accédez à HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Si DisableFileSyncNGSC est présent et est paramétré définit sur 1, ouvrez la clé et modifiez la valeur sur 0.
3. Lancer manuellement OneDrive en accédant au menu Démarrer ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.

**Réinitialiser OneDrive :**

Remarques :

- La réinitialisation de OneDrive déconnecte toutes vos connexions de synchronisation existantes (y compris de votre OneDrive personnel, s’il est configuré).
- La réinitialisation de OneDrive sur votre ordinateur n’entraîne pas de perte de fichiers ou de données.

**Pour réinitialiser OneDrive :**

1. Ouvrez une boîte de dialogue Exécuter en appuyant sur la touche Windows et sur R.
2. Tapez %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, puis appuyez sur OK. Une fenêtre Commande peut s’afficher brièvement.
3. Lancer manuellement OneDrive en accédant au menu Démarrer ![Appuyez sur la touche Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), tapez OneDrive dans la zone de recherche, puis cliquez sur l’application de bureau OneDrive.

Remarques :

- Si vous aviez choisi de ne synchroniser que quelques dossiers avant la réinitialisation, vous devrez recommencer une fois la synchronisation terminée. Pour plus d’informations, lisez  [Choisir quels dossiers OneDrive synchroniser avec votre ordinateur](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .
- Vous devrez effectuer cette opération pour votre espace OneDrive Personnel et OneDrive Entreprise.