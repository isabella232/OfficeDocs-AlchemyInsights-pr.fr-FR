---
title: PACM pour SharePoint, OneDrive et Microsoft Teams
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
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715559"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>PACM pour SharePoint, OneDrive et Microsoft Teams

Procédez comme suit pour activer la protection avancée contre les menaces :

1. Accédez à [https://protection.office.com](https://protection.office.com) et connectez-vous à l’aide d’un compte d’administrateur général ou d’administrateur de sécurité.

2. Dans le volet de navigation de gauche, sous **gestion des menaces**, sélectionnez **stratégie** de \> **pièces jointes fiables**.

3. Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams**.

4. [Créer une stratégie d’alerte d’activité](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) pour recevoir des notifications lors de la détection de fichiers malveillants.

Pour obtenir des instructions complètes, consultez cette [rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Remarque**: par conception, la protection avancée contre les menaces n’analyse pas tous les fichiers dans SharePoint Online, OneDrive entreprise ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone par un processus qui utilise l’activité de partage, l’activité des invités et des signaux de menace pour identifier les fichiers malveillants. Pour plus d’informations, consultez cette [rubrique](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
