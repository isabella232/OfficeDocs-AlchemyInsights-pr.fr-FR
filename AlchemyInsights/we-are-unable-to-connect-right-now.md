---
title: 'Problème d’activation : nous ne pouvons pas nous connecter pour le moment'
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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998150"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Résolution du message Microsoft 365 applications « Nous ne sommes pas en mesure de nous connecter pour le moment »

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour vérifier qu’ils ne bloquent pas l’accès à Internet Microsoft 365 applications. Voir [URL et plages d’adresses IP Microsoft.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Assurez-vous que les services suivants sont tous en cours d’exécution :
    - Configuration automatique des appareils connectés au réseau
    - Service de liste réseau
    - Sensibilisation de l’emplacement réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc /scannow**

Une fois cette commande terminé, redémarrez l’ordinateur.

Pour plus d’informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » lorsque vous activez Office à partir Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).