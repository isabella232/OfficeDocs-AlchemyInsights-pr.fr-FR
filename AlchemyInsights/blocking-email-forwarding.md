---
title: 726 Blocage du forwarding de courrier électronique
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059630"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocage ou déblocage du forwarding de courrier électronique

Pour activer ou désactiver le forwarding de courrier pour une boîte aux lettres spécifique, voir [Configurer le forwarding de courrier.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Au niveau du client, le contrôle du forwarding externe est effectué à l’aide de la stratégie de courrier indésirable sortant. Vous pouvez consulter la stratégie de filtrage [](https://protection.office.com/antispam) du courrier indésirable sortant à partir du Centre de sécurité et conformité ici ou à l’aide de la commande [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Si vous avez l’erreur suivante : « **550 5.7.520** Accès refusé, votre organisation n’autorise pas le forwarding externe », assurez-vous que la stratégie est configurée pour activer le forward automatique externe.

**Remarque :** Il est recommandé de conserver la fonction Deforward externe désactivée sur votre stratégie de filtrage du courrier indésirable sortant par défaut et de l’activer uniquement pour les utilisateurs qui ont besoin d’un forwarding externe en créant une stratégie personnalisée pour ces utilisateurs. Vous pouvez en savoir plus dans [la configuration du forwarding de courrier externe dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).