---
title: Permettre à un utilisateur de synchroniser un compte personnel avec le compte professionnel dans Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: ad4b64c4bb50f50d4ab9fa47bb37228dce538e6d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317276"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permettre à un utilisateur de synchroniser un compte personnel avec le compte professionnel dans Microsoft Edge

Vérifiez que vous répondez aux critères suivants :

- Enterprise State Roaming est activé dans le centre d'administration d'Azure Active Directory, ce qui nécessite un abonnement à Azure Active Directory Premium ou à Enterprise Mobility + Security (EMS). Pour plus d’informations, voir [Activer Enterprise State Roaming dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-enable).
- L’un des critères suivants ou les deux sont remplis :
    - Le service Azure Information Protection est activé pour votre client. Pour plus d’informations, consultez [Activer Microsoft Azure Rights Management à partir du Centre d’administration Microsoft 365](https://docs.microsoft.com/azure/information-protection/activate-office365).
    - La fonctionnalité Azure Active Directory Enterprise State Roaming (ESR) est activée pour n’importe quel utilisateur ou client. Pour plus d’informations, consultez [Qu’est-ce que l’itinérance d’état d’entreprise ?](https://docs.microsoft.com/azure/active-directory/devices/enterprise-state-roaming-overview).

Si AIP et ESR sont tous deux désactivés, un message d’erreur informe les utilisateurs que la synchronisation n’est pas disponible pour leurs comptes.
