---
title: Résolution Microsoft 365 applications désolés, nous avons un message de problèmes de serveur temporaires
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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744644"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Résolution du Microsoft 365 des applications « Désolé, nous avons des problèmes temporaires sur le serveur »

Remarque : si vous utilisez une version antérieure de Windows (par exemple, Windows 7 SP1, Windows Server 2008 R2), utilisez le correctif simple pour activer TLS 1.2 par défaut. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Pour plus d’informations, consultez [Mise à jour pour activer TLS 1.1 et TLS 1.2 comme protocoles sécurisés par défaut dans WinHTTP dans Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Si vous recevez ce message, essayez ce qui suit :

1. Vérifiez vos paramètres de pare-feu, de logiciel antivirus et de proxy pour confirmer qu’ils ne bloquent pas l’accès à Internet Microsoft 365 applications. Voir [URL et plages d’adresses IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Go to **Start**  >  **Run**, and then type **services.msc**. Assurez-vous que les services suivants sont tous en cours d’exécution :
    - Configuration automatique des appareils connectés au réseau
    - Service de liste réseau
    - Sensibilisation de l’emplacement réseau
    - Windows Journal des événements

Si l’un de ces services n’est pas en cours d’exécution, essayez de le démarrer. Si vous avez un problème lors du démarrage du service, exécutez la commande suivante en ouvrant une invite de commandes avec des autorisations élevées :

**sfc /scannow**

Une fois cette commande terminé, redémarrez l’ordinateur.

Pour plus d’informations, voir « Désolé, nous ne pouvons pas nous [connecter à votre compte. Veuillez réessayer ultérieurement » erreur lors de l’activation.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)