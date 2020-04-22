---
title: Correction des applications Office Désolé, nous avons un message de problèmes de serveur temporaire
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764115"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Correction des applications Office « Désolé, nous rencontrons des problèmes de serveur temporaires »

Si vous recevez ce message, procédez comme suit :

1. Vérifiez votre pare-feu, votre logiciel antivirus et vos paramètres proxy pour confirmer qu’ils ne bloquent pas l’accès Internet aux applications Office. Voir [URL et plages d’adresses IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Accédez à **Démarrer** > l'**exécution**, puis tapez **services. msc**. Assurez-vous que les services suivants sont en cours d’exécution :
    - Configuration automatique des périphériques connectés au réseau
    - Service de liste de réseaux
    - Connaissance des emplacements réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous rencontrez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc/scannow**

Une fois que cette commande est terminée, redémarrez l’ordinateur.

Pour plus d’informations, consultez [la rubrique «Désolé, nous ne pouvons pas vous connecter à votre compte. Réessayez ultérieurement» lorsque vous procédez à l’activation](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).