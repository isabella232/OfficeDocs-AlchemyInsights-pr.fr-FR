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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716170"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Correction des applications Office « nous ne parvenons pas à se connecter maintenant »

Si vous recevez ce message, procédez comme suit :

1. Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Office. Consultez la rubrique [URL et plages d’adresses IP Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accédez à **Démarrer** > l'**exécution**, puis tapez **services. msc**. Assurez-vous que les services suivants sont en cours d’exécution :
    - Configuration automatique des périphériques connectés au réseau
    - Service de liste de réseaux
    - Connaissance des emplacements réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc/scannow**

Une fois que cette commande est terminée, redémarrez l’ordinateur.

Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Veuillez réessayer plus tard» lorsque vous activez Office à partir de Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).