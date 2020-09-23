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
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="1b35e-102">Blocage ou déblocage du transfert du courrier</span><span class="sxs-lookup"><span data-stu-id="1b35e-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="1b35e-103">Pour activer ou désactiver le transfert de courrier pour une boîte aux lettres spécifique, voir [configurer le transfert du courrier](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1b35e-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="1b35e-104">Au niveau du client, le contrôle du transfert externe est réalisé à l’aide de la stratégie anti-courrier indésirable sortante.</span><span class="sxs-lookup"><span data-stu-id="1b35e-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="1b35e-105">S’il est défini sur désactivé ou automatique, il peut bloquer le transfert du courrier électronique avec le message d’erreur « 550 5.7.520 accès refusé, votre organisation n’autorise pas le transfert externe ».</span><span class="sxs-lookup"><span data-stu-id="1b35e-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="1b35e-106">Par la suite, si le transfert a été défini comme étant bloqué, il s’agit de l’erreur que vos utilisateurs verront.</span><span class="sxs-lookup"><span data-stu-id="1b35e-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="1b35e-107">Si le transfert est bloqué, vérifiez que la stratégie est configurée pour activer l’autoforward.</span><span class="sxs-lookup"><span data-stu-id="1b35e-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="1b35e-108">Vous pouvez vérifier la stratégie de filtrage du courrier indésirable sortant dans le centre de sécurité et de conformité ou en exécutant la commande Get-HostedOutboundSpamFilterPolicy | fl nom, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="1b35e-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="1b35e-109">Si vous souhaitez configurer le blocage de la fonction de transfert des redirections, la même commande vous indiquera l’état de la stratégie.</span><span class="sxs-lookup"><span data-stu-id="1b35e-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="1b35e-110">Remarque : il est recommandé de conserver le transfert automatique externe désactivé sur votre stratégie de filtrage du courrier indésirable sortant par défaut et de l’activer uniquement pour les utilisateurs qui ont besoin d’un transfert externe en créant une stratégie personnalisée pour ces utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="1b35e-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="1b35e-111">Pour plus d’informations, reportez-vous à la [configuration du transfert de messages externes dans Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="1b35e-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>