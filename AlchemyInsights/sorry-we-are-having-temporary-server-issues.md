---
title: Résolution des problèmes d'applications Microsoft 365 Désolé... Nous avons un message de problèmes de serveur temporaires
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835269"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Résolution du message des applications Microsoft 365 « Désolé, nous avons des problèmes de serveur temporaires »

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour confirmer qu'ils ne bloquent pas l'accès Internet aux applications Microsoft 365. Voir [URL et plages d'adresses IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Assurez-vous que les services suivants sont tous en cours d'exécution :
    - Configuration automatique des appareils connectés au réseau
    - Service de liste réseau
    - Sensibilisation de l'emplacement réseau
    - Windows Journal des événements

Si l'un de ces services n'est pas en cours d'exécution, essayez de le démarrer. Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc /scannow**

Une fois cette commande terminé, redémarrez l'ordinateur.

Pour plus d'informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » erreur lors de l'activation.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)