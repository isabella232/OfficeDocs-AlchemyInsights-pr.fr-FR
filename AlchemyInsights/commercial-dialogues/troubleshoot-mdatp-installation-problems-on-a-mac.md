---
title: Résoudre les problèmes d’installation MDATP sur un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091027"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Résoudre les problèmes d’installation MDATP sur un Mac

Si l’installation manuelle échoue, la page **Résumé** de l’Assistant Installation affiche l’erreur suivante :

« Une erreur s’est produite lors de l’installation. Le programme d’installation a rencontré une erreur qui a provoqué l’échec de l’installation. Contactez le fabricant du logiciel pour obtenir de l’aide. »

Pour les déploiements mdm, la page affiche également un échec d’installation générique.

Bien que nous n’affichions pas d’erreurs exactes pour les utilisateurs finaux, nous tenez un fichier journal avec la progression de l’installation, dans **/Library/Logs/Microsoft/mdatp/install.log**. Chaque session d’installation s’y connecte. Pour n’en sortie que la dernière session d’installation, utilisez `sed` .

Pour plus d’informations, voir Résoudre les problèmes [d’installation de Microsoft Defender ATP pour Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
