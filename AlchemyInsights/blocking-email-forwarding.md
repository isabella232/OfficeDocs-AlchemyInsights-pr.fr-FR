---
title: 726 blocage du transfert du courrier électronique
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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478321"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocage ou déblocage du transfert du courrier

Pour activer ou désactiver le transfert de courrier pour une boîte aux lettres spécifique, voir [configurer le transfert du courrier](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Au niveau du client, le contrôle du transfert externe est réalisé à l’aide de la stratégie de courrier indésirable sortant. Vous pouvez vérifier la stratégie de filtrage du courrier indésirable sortant dans le centre de sécurité et de conformité [ici](https://protection.office.com/antispam) ou à l’aide de la [commande Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Si vous obtenez l’erreur suivante : **« 550 5.7.520 accès refusé, votre organisation n’autorise pas le transfert externe »**, vérifiez que la stratégie est configurée pour activer le transfert automatique externe.

**Remarque :** Il est recommandé de conserver le transfert automatique externe désactivé sur votre stratégie de filtrage du courrier indésirable sortant par défaut et de l’activer uniquement pour les utilisateurs qui ont besoin d’un transfert externe en créant une stratégie personnalisée pour ces utilisateurs. Pour plus d’informations, reportez-vous à la [configuration du transfert de messages externes dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).