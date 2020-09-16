---
title: Corriger l’erreur 0x8004de40 dans OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745128"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Corriger l’erreur 0x8004de40 dans OneDrive

Si vous recevez une erreur 0x8004de40 avec OneDrive :

- Redémarrez l’ordinateur concerné en étant connecté à votre domaine d’annuaire acitve.
- Si un redémarrage ne résout pas le problème, Déjoignez et rejoignez votre appareil à partir d’Azure AD. 

**Remarque**: vous devez être sur votre réseau d’entreprise tout en effectuant ces étapes. N’effectuez pas ces étapes Lorsque vous ne parvenez pas à vous connecter à votre infrastructure d’entreprise (par exemple, lors de vos déplacements). 

- Ouvrez une invite de commandes avec élévation de privilèges. 
- Pour ouvrir une invite de commandes avec élévation de privilèges, cliquez sur- **Démarrer**, cliquez avec le bouton droit sur **invite de commandes**, puis cliquez sur **exécuter en tant qu’administrateur**.
- Tapez *dsregcmd/Leave* , puis appuyez sur **entrée**.
- Lorsque vous avez terminé, tapez *dsregcmd/Join* , puis appuyez sur **entrée**.
- Lorsque vous avez terminé, fermez l’invite de commandes.
- Redémarrez l’ordinateur, puis connectez-vous à OneDrive.