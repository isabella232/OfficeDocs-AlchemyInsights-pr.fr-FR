---
title: "Problème d'activation : nous ne pouvons pas nous connecter pour le moment"
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
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806440"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Résolution du message des applications Microsoft 365 « Nous ne pouvons pas nous connecter pour le moment »

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour confirmer qu'ils ne bloquent pas l'accès Internet aux applications Microsoft 365. Voir [URL et plages d'adresses IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Assurez-vous que les services suivants sont tous en cours d'exécution :
    - Configuration automatique des appareils connectés au réseau
    - Service de liste réseau
    - Sensibilisation de l'emplacement réseau
    - Windows Journal des événements

Si l'un de ces services n'est pas en cours d'exécution, essayez de le démarrer. Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc /scannow**

Une fois cette commande terminé, redémarrez l'ordinateur.

Pour plus d'informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » lorsque vous activez Office à partir de Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)