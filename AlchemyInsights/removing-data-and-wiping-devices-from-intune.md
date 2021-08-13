---
title: Suppression des données et réinitialisation d’appareils dans Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922218"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Suppression des données et réinitialisation d’appareils dans Intune

Les actions à distance Mise hors service et Réinitialisation peuvent être utilisées pour supprimer les données de l'entreprise gérées par Intune ou pour effectuer une réinitialisation aux paramètres d'usine et rétablir les paramètres par défaut de l'appareil.

1. Connectez-vous à la gestion des appareils Microsoft 365 et accédez à **Appareils** > **Tous les appareils**.
2. Sélectionnez l’appareil que vous voulez réinitialiser.
3. Sélectionnez le type de réinitialisation à distance que vous voulez effectuer. La mise hors service supprime uniquement les informations de l’organisation, tandis que les réinitialisations complètes restaurent les paramètres par défaut de l’appareil.
4. Cliquez sur **Oui** pour confirmer. Jusqu’à la fin de la réinitialisation, l’état d’action de l’appareil indique comme *Mise hors service en attente*.
    Une fois l’action terminée, vous ne verrez plus l’appareil mobile dans la liste des appareils gérés.

> [!NOTE]
> Les données de l’entreprise ne peuvent pas être supprimées des appareils joints à Azure AD. 

Pour plus d’informations sur l’effet des actions de Mise hors service et Réinitialisation, notamment les éléments conservés et les éléments supprimés, consultez la documentation suivante :

- [Supprimez des appareils à l’aide d’un effacement, d’une mettre hors service ou d’un programme d’inscription manuelle de l'appareil](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Effacement des données d’entreprise provenant d’applications gérées par Intune uniquement](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Effacer toutes les données d’un appareil macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).