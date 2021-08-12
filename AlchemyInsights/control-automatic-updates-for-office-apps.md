---
title: Contrôler les mises à jour automatiques pour les applications Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929879"
---
# <a name="control-automatic-updates-for-office-apps"></a>Contrôler les mises à jour automatiques pour les applications Office

Par défaut, les mises à jour des applications Office sont téléchargées automatiquement et appliquées en arrière-plan, sans aucune intervention de l’utilisateur. Toutefois, les administrateurs peuvent contrôler la manière dont les mises à jour sont appliquées à l’aide des paramètres de mise à jour d’Office. Les paramètres de mise à jour permettent aux administrateurs d’activer ou de désactiver les mises à jour automatiques, d’afficher ou de masquer le bouton **Mettre à jour maintenant** dans Office, définir des échéances de mise à jour, etc. Pour plus d'informations, consultez :

- [Définir les paramètres de mise à jour pour Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Les mises à jour automatiques pour Office ne sont pas activées](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Définir la façon dont Office est mis à jour après l’installation](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Pour passer en revue les paramètres de mises à jour existants appliqués à un ordinateur client, procédez comme suit :

1. Ouvrez l’Éditeur du registre en accédant à **Démarrer** > **Exécuter** > **regedit**.
2. Accédez à l’emplacement suivant et passez en revue les paramètres de mise à jour d’Office :  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Remarque**  si la clé OfficeMgmtCOM est activée, vous pouvez afficher le message « Les mises à jour sont gérées par votre administrateur système » dans **Office** > **Compte** > **Mises à jour d’Office**. Pour plus d’informations, consultez [Gestion des mises à jour vers Microsoft 365 Apps avec Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  