---
title: Activer la protection avancée contre les menaces Office 365 pour SharePoint, OneDrive et Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703424"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activer Office 365 protection avancée contre les menaces pour SharePoint Online, OneDrive et Microsoft teams

1. Accédez à https://protection.office.com et connectez-vous.
2. Choisissez**pièces jointes fiables**pour la**stratégie** > de **gestion** > des menaces.
3. Sélectionnez Activer la protection avancée contre **les menaces pour SharePoint, OneDrive et Microsoft teams**, puis cliquez sur **Enregistrer**.
4. Recommandation En tant qu’administrateur général ou administrateur SharePoint Online, exécutez la cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) avec le paramètre **DisallowInfectedFileDownload** défini sur *true*.
5. Recommandation [Configurez les alertes](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pour les fichiers détectés.

> [!NOTE]
> La fonctionnalité ATP va analyser tous les fichiers dans SharePoint Online, OneDrive ou Microsoft Teams. Les fichiers sont analysés de manière asynchrone, via un processus qui utilise des événements d’activité de partage et d’invité, ainsi que des méthodes heuristiques intelligentes et des signaux de menace pour identifier les fichiers malveillants. Voir [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams) (en anglais).