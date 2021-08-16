---
title: Problèmes d’installation de Microsoft Defender sur Mac ou Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013242"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Problèmes d’installation de Microsoft Defender sur Mac ou Linux

**Mac**

- Assurez-vous que la configuration requise est respectée avant d’installer Microsoft Defender ATP pour Mac. Pour plus d’informations, voir [Installation de Microsoft Defender ATP pour Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Examinez les informations du fichier : « /Library/Logs/Microsoft/mdatp/install.log ».

**Linux**

- Assurez-vous que la configuration requise est respectée avant d’installer Microsoft Defender ATP pour Linux. Pour plus d'informations, voir [Comment installer MDATP pour Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Pour vérifier que le service MDATP est en cours d’exécution, voir [Échec de l’installation](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).  
    Pour résoudre les problèmes si le service n’est pas en cours d’exécution, consultez [Étapes de résolution des problèmes si le service mdatp n’est pas en cours d’exécution](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Pour connaître la procédure de vérification de la configuration du client, qui vérifie l’intégrité du produit, et d’exécution d’un test de détection sur le fichier texte EICAR, voir [Configuration du client](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Remarque** Pour obtenir la liste des systèmes de fichiers pris en charge pour l’activité à l’accès, voir [Microsoft Defender ATP pour Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).