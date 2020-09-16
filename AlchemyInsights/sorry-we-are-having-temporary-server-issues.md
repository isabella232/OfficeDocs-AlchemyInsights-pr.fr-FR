---
title: Résolution des applications Microsoft 365 Désolé, un message de problèmes de serveur temporaire s’affiche.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758243"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Résolution des applications Microsoft 365 les applications « Désolé, nous rencontrons des problèmes de serveur temporaires »

Si vous recevez ce message, procédez comme suit :

1. Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Microsoft 365. Voir [URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accédez à **Démarrer**l'  >  **exécution**, puis tapez **services. msc**. Assurez-vous que les services suivants sont en cours d’exécution :
    - Configuration automatique des périphériques connectés au réseau
    - Service de liste de réseaux
    - Connaissance des emplacements réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc/scannow**

Une fois que cette commande est terminée, redémarrez l’ordinateur.

Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Réessayez ultérieurement» lorsque vous procédez à l’activation](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).