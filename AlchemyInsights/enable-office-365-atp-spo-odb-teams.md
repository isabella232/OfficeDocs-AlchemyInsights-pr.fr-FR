---
title: Activer la protection avancée contre les menaces Office 365 pour SharePoint, OneDrive et Microsoft teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801045"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activation de Microsoft Defender pour Office 365 pour SharePoint Online, OneDrive et Microsoft teams

1. Accédez à https://protection.office.com et connectez-vous.
2. Choisissez **Threat management**  >  **Policy**  >  **pièces jointes fiables** pour la stratégie de gestion des menaces.
3. Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams** , puis cliquez sur **Enregistrer** .
4. Recommandation En tant qu’administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** défini sur *true* .
5. Recommandation [Configurez les alertes](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pour les fichiers détectés.

> [!NOTE]
> La fonctionnalité ATP va analyser tous les fichiers dans SharePoint Online, OneDrive ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone, via un processus qui utilise des événements d’activité de partage et d’invité, ainsi que des méthodes heuristiques intelligentes et des signaux de menace pour identifier les fichiers malveillants. Voir [ATP pour SharePoint, OneDrive et Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).