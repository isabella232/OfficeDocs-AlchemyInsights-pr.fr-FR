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
ms.openlocfilehash: 4c246fcc9ef0e3a79c3e68be491e3e7f5c6edb0b
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603249"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Permettre à un utilisateur de synchroniser un compte personnel avec le compte professionnel dans Microsoft Edge

Vérifiez que vous répondez aux critères suivants :

- Enterprise State Roaming est activée dans le centre d'administration d'Azure Active Directory, ce qui nécessite un abonnement à Azure Active Directory Premium ou à Enterprise Mobility + Security (EMS). Pour plus d’informations, consultez [Activer Enterprise State Roaming dans Azure Active Directory](/azure/active-directory/devices/enterprise-state-roaming-enable).
- L’un des critères suivants ou les deux sont remplis :
    - Le service Azure Information Protection est activé pour votre client. Pour plus d’informations, consultez [Activer Microsoft Azure Rights Management à partir du Centre d’administration Microsoft 365](/azure/information-protection/activate-office365).
    - La fonctionnalité Azure Active Directory Enterprise State Roaming (ESR) est activée pour n’importe quel utilisateur ou client. Pour plus d’informations, consultez [Qu’est-ce que l’itinérance d’état d’entreprise ?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Si AIP et ESR sont tous deux désactivés, un message d’erreur informe les utilisateurs que la synchronisation n’est pas disponible pour leurs comptes.
