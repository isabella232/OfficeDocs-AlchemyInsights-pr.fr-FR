---
title: Paramètres de démarrage dans Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909824"
---
# <a name="startup-settings-in-windows-10"></a>Paramètres de démarrage dans Windows 10

**Modifier les applications qui s’exécutent automatiquement au démarrage**

1. Go to [Paramètres > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Assurez-vous que toutes les applications que vous souhaitez exécuter au démarrage sont **allumées.**

**Ajouter une application à exécuter automatiquement au démarrage**

1. Cliquez ou appuyez **sur Démarrer** et recherchez l’application que vous souhaitez exécuter au démarrage.

2. Cliquez avec le bouton droit sur l’application, cliquez **sur Plus,** puis cliquez **sur Ouvrir l’emplacement du fichier.** Cela ouvre l’emplacement où le raccourci vers l’application est enregistré. S’il n’existe aucune option pour ouvrir l’emplacement du fichier, cela signifie que l’application ne peut pas s’exécuter au démarrage.

3. Une fois l’emplacement du fichier ouvert, **appuyez** sur Windows de logo + R , tapez **shell:startup,** puis cliquez sur **OK**. Le dossier De démarrage s’ouvre.

4. Copiez et collez le raccourci vers l’application à partir de l’emplacement du fichier dans le dossier De démarrage.

**Options de démarrage avancées (y compris le mode Coffre, les paramètres UEFI et le démarrage à partir d’un autre appareil)**

1. Enregistrez votre travail et fermez les documents ouverts, car ces étapes redémarreront votre PC.

2. Go to [Paramètres > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).

3. Sous **Démarrage avancé,** cliquez sur **Redémarrer maintenant.** 

4. Après le redémarrage de votre PC sur l’écran Choisir une option :

    - Pour démarrer à partir d’un appareil tel qu’un lecteur USB, cliquez **sur Utiliser un appareil.**

    - Pour entrer les paramètres UEFI (parfois appelés configuration du BIOS), cliquez sur Résoudre les problèmes > options avancées > du **microprogramme UEFI Paramètres**. 

    - Pour entrer Coffre mode de démarrage ou modifier les paramètres de démarrage avancés, cliquez sur Résoudre les problèmes > Options avancées **> démarrage Paramètres,** puis cliquez sur **Redémarrer.** Vous pouvez être invité à entrer votre clé de récupération [BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Après le redémarrage de votre PC, cliquez sur le paramètre de démarrage que vous souhaitez utiliser.