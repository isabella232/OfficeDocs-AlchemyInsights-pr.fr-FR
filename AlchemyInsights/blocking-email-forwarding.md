---
title: Bloquer ou débloquer le forwarding automatique du courrier externe
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315872"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Bloquer ou débloquer le forwarding automatique du courrier électronique

Pour activer ou désactiver le forwarding de courrier pour une boîte aux lettres spécifique, voir [Configurer le forwarding de courrier.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Les administrateurs peuvent contrôler le forwarding externe pour l’organisation à l’aide de [stratégies de courrier indésirable sortant.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Vous gérez les stratégies de courrier indésirable sortant dans le portail Microsoft 365 Defender à l’aide de la <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) dans Exchange Online PowerShell.

Si vous recevez l’erreur suivante : « **550 5.7.520** Accès refusé, votre organisation n’autorise pas le forwarding externe » , assurez-vous que la stratégie est configurée pour activer les messages externes à transmis automatiquement.

**Remarque**: nous avons recommandé la valeur par défaut **Automatic - System controlled** for the **Automatic forwarding rules** setting in your default outbound spam filter policy (automatic external forwarding is blocked; internal automatic forwarding still works). Vous devez créer des stratégies personnalisées de filtrage du courrier indésirable sortant et utiliser la valeur **On - Le forwarding** est activé uniquement pour les utilisateurs qui ont besoin d’un filtrage automatique des messages externes. Pour plus d’informations, voir [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
