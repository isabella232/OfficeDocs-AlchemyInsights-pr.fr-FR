---
title: 'Problème d’activation : nous ne pouvons pas vous connecter pour le moment'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628240"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Correction des applications Office « nous ne parvenons pas à se connecter maintenant »

Si vous recevez ce message, procédez comme suit :

1. Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Office. Voir [URL et plages d’adresses IP Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accédez à **Démarrer** > l'**exécution**, puis tapez **services. msc**. Assurez-vous que les services suivants sont en cours d’exécution :
    - Configuration automatique des périphériques connectés au réseau
    - Service de liste de réseaux
    - Connaissance des emplacements réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc/scannow**

Une fois que cette commande est terminée, redémarrez l’ordinateur.

Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Veuillez réessayer plus tard» lorsque vous activez Office à partir d’Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).