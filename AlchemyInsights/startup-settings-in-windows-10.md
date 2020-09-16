---
title: Paramètres de démarrage dans Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751133"
---
# <a name="startup-settings-in-windows-10"></a>Paramètres de démarrage dans Windows 10

**Modifier les applications qui s’exécutent automatiquement au démarrage**

1. Accédez à [paramètres > Apps > démarrage](ms-settings:startupapps?activationSource=GetHelp).

2. Assurez-vous que toutes les applications que vous souhaitez exécuter au démarrage **sont activées.**

**Ajouter une application pour qu’elle s’exécute automatiquement au démarrage**

1. Cliquez ou appuyez sur **Démarrer** et recherchez l’application que vous souhaitez exécuter au démarrage.

2. Cliquez avec le bouton droit sur l’application, cliquez sur **plus**, puis sur **ouvrir l’emplacement du fichier**. Cette action ouvre l’emplacement où le raccourci vers l’application est enregistré. S’il n’existe pas d’option pour l’emplacement des fichiers ouverts, cela signifie que l’application ne peut pas être exécutée au démarrage.

3. Une fois l’emplacement du fichier ouvert, appuyez sur la **touche du logo Windows + R**, tapez **Shell : Startup**, puis cliquez sur **OK**. Le dossier démarrage s’ouvre.

4. Copiez et collez le raccourci vers l’application à partir de l’emplacement du fichier vers le dossier de démarrage.

**Options de démarrage avancées (y compris le mode sans échec, les paramètres UEFI et le démarrage à partir d’un autre périphérique)**

1. Enregistrez votre travail et fermez tous les documents ouverts, étant donné que ces étapes redémarreront votre PC.

2. Accédez à [paramètres > mise à jour & la récupération de la sécurité >](ms-settings:recovery?activationSource=GetHelp).

3. Sous **démarrage avancé**, cliquez sur **redémarrer maintenant**. 

4. Après que votre PC a redémarré sur l’écran choisir une option, procédez comme suit :

    - Pour démarrer à partir d’un appareil comme un lecteur USB, cliquez sur **utiliser un appareil**.

    - Pour entrer les paramètres UEFI (parfois appelés configuration du BIOS), cliquez sur **Troubleshoot > Advanced options > firmware UEFI Settings**. 

    - Pour entrer en mode sans échec ou modifier les paramètres de démarrage avancés, cliquez sur **Troubleshoot > Advanced options > paramètres de démarrage**, puis sur **redémarrer**. Vous serez peut-être invité à entrer votre [clé de récupération BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Une fois que votre PC a redémarré, cliquez sur le paramètre de démarrage que vous souhaitez utiliser.