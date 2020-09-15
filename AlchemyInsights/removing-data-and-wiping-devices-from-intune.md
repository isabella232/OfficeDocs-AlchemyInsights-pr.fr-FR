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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701281"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Suppression des données et réinitialisation d’appareils dans Intune

Les actions à distance Mise hors service et Réinitialisation peuvent être utilisées pour supprimer les données de l'entreprise gérées par Intune ou pour effectuer une réinitialisation aux paramètres d'usine et rétablir les paramètres par défaut de l'appareil.

1. Connectez-vous à la gestion des appareils Microsoft 365 et accédez à **Appareils** > **Tous les appareils**.
2. Sélectionnez l’appareil que vous voulez réinitialiser.
3. Sélectionnez le type de réinitialisation à distance que vous voulez effectuer. La mise hors service supprime uniquement les informations de l’organisation, tandis que les réinitialisations complètes restaurent les paramètres par défaut de l’appareil.
4. Cliquez sur **Oui** pour confirmer. Jusqu’à la fin de la réinitialisation, l’état d’action de l’appareil indique comme Mise hors service en attente.</br>
    Une fois l’action terminée, vous ne verrez plus l’appareil mobile dans la liste des appareils gérés.

**Remarque** les données de l’entreprise ne peuvent pas être supprimées des appareils joints à Azure AD.

Pour plus d’informations sur l’effet des actions de Mise hors service et Réinitialisation, notamment les éléments conservés et les éléments supprimés, consultez [Supprimer des appareils à l’aide de l’opération de réinitialisation, de mise hors service ou de désinscription manuelle de l’appareil](https://docs.microsoft.com/intune/devices-wipe).

Pour effacer toutes les données d’un appareil macOS, consultez [Effacer toutes les données d’un appareil macOS](https://docs.microsoft.com/intune/device-erase).