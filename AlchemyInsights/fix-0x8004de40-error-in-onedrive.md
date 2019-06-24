---
title: Corriger l’erreur 0x8004de40 dans OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133975"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corriger l’erreur 0x8004de40 dans OneDrive

Si vous recevez une erreur 0x8004de40 avec OneDrive:

- Redémarrez l’ordinateur concerné en étant connecté à votre domaine d’annuaire acitve.
- Si un redémarrage ne résout pas le problème, Déjoignez et rejoignez votre appareil à partir d’Azure AD. 

**Remarque**: vous devez être sur votre réseau d’entreprise tout en effectuant ces étapes. N’effectuez pas ces étapes Lorsque vous ne parvenez pas à vous connecter à votre infrastructure d’entreprise (par exemple, lors de vos déplacements). 

- Ouvrez une invite de commandes avec élévation de privilèges. 
- Pour ouvrir une invite de commandes avec élévation de privilèges, cliquez sur- **Démarrer**, cliquez avec le bouton droit sur **invite de commandes**, puis cliquez sur **exécuter en tant qu’administrateur**.
- Tapez *dsregcmd/Leave* , puis appuyez sur **entrée**.
- Lorsque vous avez terminé, tapez *dsregcmd/Join* , puis appuyez sur **entrée**.
- Lorsque vous avez terminé, fermez l’invite de commandes.
- Redémarrez l’ordinateur, puis connectez-vous à OneDrive.