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
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="2f5f3-102">Blocage ou déblocage du transfert du courrier</span><span class="sxs-lookup"><span data-stu-id="2f5f3-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="2f5f3-103">Pour activer ou désactiver le transfert de courrier pour une boîte aux lettres spécifique, voir [configurer le transfert du courrier](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="2f5f3-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="2f5f3-104">Au niveau du client, le contrôle du transfert externe est réalisé à l’aide de la stratégie de courrier indésirable sortant.</span><span class="sxs-lookup"><span data-stu-id="2f5f3-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="2f5f3-105">Vous pouvez vérifier la stratégie de filtrage du courrier indésirable sortant dans le centre de sécurité et de conformité [ici](https://protection.office.com/antispam) ou à l’aide de la [commande Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="2f5f3-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="2f5f3-106">Si vous obtenez l’erreur suivante : **« 550 5.7.520 accès refusé, votre organisation n’autorise pas le transfert externe »**, vérifiez que la stratégie est configurée pour activer le transfert automatique externe.</span><span class="sxs-lookup"><span data-stu-id="2f5f3-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="2f5f3-107">**Remarque :** Il est recommandé de conserver le transfert automatique externe désactivé sur votre stratégie de filtrage du courrier indésirable sortant par défaut et de l’activer uniquement pour les utilisateurs qui ont besoin d’un transfert externe en créant une stratégie personnalisée pour ces utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="2f5f3-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="2f5f3-108">Pour plus d’informations, reportez-vous à la [configuration du transfert de messages externes dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="2f5f3-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>