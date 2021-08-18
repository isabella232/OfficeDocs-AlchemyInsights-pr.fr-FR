---
title: Activer Office 365 atp pour SharePoint, OneDrive et Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332157"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activez Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive et Microsoft Teams

1. Accédez à https://protection.office.com et connectez-vous.
2. Choose **Threat management**  >  **Policy** Coffre  >  **Attachments**.
3. Sélectionnez **Activer Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams,** puis cliquez sur **Enregistrer.**
4. (Recommandé) En tant qu’administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** définie sur *true*.
5. (Recommandé) [Configurer des alertes pour](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) les fichiers détectés.

**Remarque**: Microsoft Defender pour Office 365 n’analyse pas tous les fichiers dans SharePoint Online, OneDrive ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone, par le biais d’un processus qui utilise des événements de partage et d’activité invité, ainsi que des signaux heuristiques intelligents et des signaux de menace pour identifier les fichiers malveillants. Consultez [Microsoft Defender pour Office 365 pour SharePoint, OneDrive et Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
