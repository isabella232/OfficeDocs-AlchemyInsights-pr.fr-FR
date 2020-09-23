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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219853"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blocage ou déblocage du transfert du courrier

Pour activer ou désactiver le transfert de courrier pour une boîte aux lettres spécifique, voir [configurer le transfert du courrier](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Au niveau du client, le contrôle du transfert externe est réalisé à l’aide de la stratégie anti-courrier indésirable sortante. S’il est défini sur désactivé ou automatique, il peut bloquer le transfert du courrier électronique avec le message d’erreur « 550 5.7.520 accès refusé, votre organisation n’autorise pas le transfert externe ». Par la suite, si le transfert a été défini comme étant bloqué, il s’agit de l’erreur que vos utilisateurs verront.

Si le transfert est bloqué, vérifiez que la stratégie est configurée pour activer l’autoforward. Vous pouvez vérifier la stratégie de filtrage du courrier indésirable sortant dans le centre de sécurité et de conformité ou en exécutant la commande Get-HostedOutboundSpamFilterPolicy | fl nom, AutoForwardingMode. Si vous souhaitez configurer le blocage de la fonction de transfert des redirections, la même commande vous indiquera l’état de la stratégie.

Remarque : il est recommandé de conserver le transfert automatique externe désactivé sur votre stratégie de filtrage du courrier indésirable sortant par défaut et de l’activer uniquement pour les utilisateurs qui ont besoin d’un transfert externe en créant une stratégie personnalisée pour ces utilisateurs. Pour plus d’informations, reportez-vous à la [configuration du transfert de messages externes dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).