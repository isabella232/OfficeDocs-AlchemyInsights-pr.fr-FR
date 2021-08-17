---
title: Activer Coffre pièces jointes pour SharePoint Online, OneDrive et Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894461"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Activer Coffre pièces jointes pour SharePoint Online, OneDrive et Microsoft Teams

1. À l’aide de vos informations d’identification d’administrateur global ou d’administrateur de sécurité, ouvrez le portail Microsoft 365 Defender à l’adresse , puis allez à Stratégies & règles stratégies de menace Coffre pièces jointes dans la <https://security.microsoft.com> section  \>  \> **Stratégies** 

   Pour aller directement à la page **Coffre pièces jointes,** utilisez <https://security.microsoft.com/safeattachmentv2> .

2. Dans la page **Coffre pièces jointes,** cliquez **sur Paramètres globaux.**
3. Dans le volant qui s’affiche, sélectionnez Activer Microsoft Defender pour Office 365 pour **SharePoint, OneDrive** et Microsoft Teams, puis sélectionnez **Enregistrer.**

    > [!TIP]
    >
    > Pour améliorer la protection des pièces jointes de Coffre, SharePoint, OneDrive et Microsoft Teams :
    >
    > - Pour empêcher les utilisateurs de télécharger des fichiers malveillants, utilisez la valeur du paramètre `$true` *DisallowInfectedFileDownload* sur la cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** dans SharePoint Online PowerShell. Pour plus d’informations, voir Utiliser SharePoint Online PowerShell pour empêcher les utilisateurs de [télécharger des fichiers malveillants.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Créer une stratégie d’alerte pour les fichiers détectés](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Pour plus d’informations, [voir Coffre Attachments for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
