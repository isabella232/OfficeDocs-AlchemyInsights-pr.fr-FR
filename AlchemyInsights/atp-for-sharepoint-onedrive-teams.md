---
title: Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 0d0fff3e699d46af2a19a8ad60696b824bafa109
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314960"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams

Suivez ces étapes pour activer Microsoft Defender pour Office 365 :

1. Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.

2. Dans le volet de navigation gauche sous **Gestion des menaces,** choisissez **Stratégie** Coffre \> **pièces jointes**.

3. Sélectionnez **Activer Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams**.

4. [Créez une stratégie d’alerte d’activité](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) pour recevoir des notifications lorsque nous détectons des fichiers malveillants.

Pour obtenir des instructions complètes, consultez cette Coffre pièces jointes pour [SharePoint, OneDrive et Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Remarque**: Par conception, Microsoft Defender pour Office 365 n’analyse pas chaque fichier dans SharePoint Online, OneDrive Entreprise ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone par un processus qui utilise l’activité de partage, l’activité des invités et les signaux de menace pour identifier les fichiers malveillants. Pour plus d’informations, [voir Coffre attachments for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
