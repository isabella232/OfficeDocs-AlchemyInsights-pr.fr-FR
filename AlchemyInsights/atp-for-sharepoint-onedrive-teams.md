---
title: Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams
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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543575"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams

Suivez ces étapes pour activer Microsoft Defender pour Office 365 :

1. Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.

2. Dans le volet de navigation gauche sous **Gestion des menaces,** choisissez **Pièces** \> **jointes sécurisées de stratégie.**

3. Sélectionnez **Activer Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams**.

4. [Créez une stratégie d’alerte d’activité](/microsoft-365/compliance/create-activity-alerts) pour recevoir des notifications lorsque nous détectons des fichiers malveillants.

Pour obtenir des instructions complètes, voir l’étape Activer les pièces [jointes sécurisées pour SharePoint, OneDrive et Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Remarque**: Par conception, Microsoft Defender pour Office 365 n’analyse pas chaque fichier dans SharePoint Online, OneDrive Entreprise ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone par un processus qui utilise l’activité de partage, l’activité des invités et les signaux de menace pour identifier les fichiers malveillants. Pour plus d’informations, [voir Pièces jointes SharePoint, OneDrive et Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
