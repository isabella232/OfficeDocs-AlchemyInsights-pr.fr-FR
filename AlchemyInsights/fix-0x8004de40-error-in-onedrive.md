---
title: Corriger 0x8004de40'erreur dans OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649746"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corriger 0x8004de40'erreur dans OneDrive

Si vous exécutez Windows 7 et recevez cette erreur, mettez à jour pour activer [TLS 1.1 et TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)en tant que protocoles sécurisés par défaut dans WinHTTP dans Windows.

Si vous exécutez Windows 10 et que vous recevez une erreur 0x8004de40 avec OneDrive :

- Redémarrez l’ordinateur affecté lorsque vous êtes connecté à votre domaine Acitve Directory.
- Si un redémarrage ne corrige pas le problème, déjoinez-vous et rejoignez votre appareil à partir d’Azure AD. 

**Remarque**: vous devez être sur votre réseau d’entreprise lors de ces étapes. N’effectuez pas ces étapes lorsque vous n’êtes pas connecté à votre infrastructure d’entreprise (par exemple, en déplacement). 

1. Ouvrez une invite de commandes avec élévation de niveau élevé en sélectionnant **Démarrer,** cliquez avec le bouton droit sur Invite de **commandes,** puis **sélectionnez Exécuter en tant qu’administrateur.**

1. Tapez *dsregcmd /leave et* appuyez sur **Entrée**.

1. Lorsque vous terminez, *tapez dsregcmd /join* et appuyez sur **Entrée**.

1. Lorsque vous terminez, fermez l’invite de commandes.

1. Redémarrez l’ordinateur et connectez-vous à OneDrive.