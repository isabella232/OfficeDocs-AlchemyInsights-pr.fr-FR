---
title: Activer Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive et Microsoft Teams
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735812"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activer Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive et Microsoft Teams

1. À l’aide de vos informations d’identification d’administrateur général ou d’administrateur de sécurité, connectez-vous au Centre de sécurité et [conformité Office 365.](https://protection.office.com/)
2. Sélectionnez **Gestion des menaces** dans le volet gauche, puis sélectionnez **Pièces**  >  [jointes sécurisées de stratégie.](https://protection.office.com/safeattachment)
3. Sélectionnez **Activer Microsoft Defender pour Office 365 pour SharePoint, OneDrive** et Microsoft Teams, puis sélectionnez **Enregistrer.**
    > [!TIP]
    >
    > - En tant qu’administrateur général ou administrateur SharePoint Online, exécutez l’cmdlet PowerShell suivante avec le paramètre **DisallowInfectedFileDownload** définie sur *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurer des alertes pour les fichiers détectés](https://go.microsoft.com/fwlink/?linkid=2092110)

Pour plus d’informations, [voir Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
