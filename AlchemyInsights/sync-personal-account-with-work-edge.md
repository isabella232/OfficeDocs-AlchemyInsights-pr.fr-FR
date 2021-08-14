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
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54009049"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permettre à un utilisateur de synchroniser un compte personnel avec le compte professionnel dans Microsoft Edge

Vérifiez que vous répondez aux critères suivants :

- Enterprise State Roaming est activé dans le centre d'administration d'Azure Active Directory, ce qui nécessite un abonnement à Azure Active Directory Premium ou à Enterprise Mobility + Security (EMS). Pour plus d’informations, voir [Activer Enterprise State Roaming dans Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- L’un des critères suivants ou les deux sont remplis :
    - Le service Azure Information Protection est activé pour votre client. Pour plus d’informations, consultez [Activer Microsoft Azure Rights Management à partir du Centre d’administration Microsoft 365](/azure/information-protection/activate-office365).
    - La fonctionnalité Azure Active Directory Enterprise State Roaming (ESR) est activée pour n’importe quel utilisateur ou client. Pour plus d’informations, consultez [Qu’est-ce que l’itinérance d’état d’entreprise ?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Si AIP et ESR sont tous deux désactivés, un message d’erreur informe les utilisateurs que la synchronisation n’est pas disponible pour leurs comptes.
