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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568626"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Résoudre les problèmes d’installation MDATP sur un Mac

En cas d’échec de l’installation manuelle, la page **Résumé** de l’Assistant Installation affiche l’erreur suivante :

« Une erreur s’est produite lors de l’installation. Le programme d’installation a rencontré une erreur qui a provoqué l’échec de l’installation. Contactez le fabricant du logiciel pour obtenir de l’aide. »

Pour les déploiements mdm, la page affiche également un échec d’installation générique.

Bien que nous n’affichions pas d’erreurs exactes pour les utilisateurs finaux, nous tenez un fichier journal avec la progression de l’installation, dans **/Library/Logs/Microsoft/mdatp/install.log**. Chaque session d’installation s’y connecte. Pour n’en sortie que la dernière session d’installation, utilisez `sed` .

Pour en savoir plus, voir Résoudre les problèmes [d’installation de Microsoft Defender ATP pour Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
