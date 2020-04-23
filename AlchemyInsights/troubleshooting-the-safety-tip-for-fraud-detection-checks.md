---
title: Dépannage du Conseil de sécurité pour les vérifications de détection de fraude
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759510"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="7ed58-102">Dépannage du Conseil de sécurité pour les vérifications de détection de fraude</span><span class="sxs-lookup"><span data-stu-id="7ed58-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="7ed58-103">Si vous recevez un Conseil de sécurité indiquant « l’échec de nos vérifications de détection de fraude par l’expéditeur et peut ne pas être celui qu’il semble être », l’expéditeur n’a pas réussi à transmettre les contrôles d’authentification DKIM ou SPF.</span><span class="sxs-lookup"><span data-stu-id="7ed58-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="7ed58-104">Pour résoudre ce cas, la meilleure méthode consiste à autoriser l’expéditeur à s’autoriser.</span><span class="sxs-lookup"><span data-stu-id="7ed58-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="7ed58-105">Si l’expéditeur est envoyé en votre nom, vous devez l’autoriser en ajoutant l’adresse IP de l’expéditeur à votre enregistrement SPF.</span><span class="sxs-lookup"><span data-stu-id="7ed58-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="7ed58-106">Pour plus d’informations, reportez-vous à [la rubrique Troubleshooting the Red (suspect) Safety Tip for fraude DETECTION checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="7ed58-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="7ed58-107">Voici quelques autres liens qui peuvent vous aider :</span><span class="sxs-lookup"><span data-stu-id="7ed58-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="7ed58-108">Comment Microsoft utilise SPF (Sender Policy Framework) pour éviter l’usurpation d’identité</span><span class="sxs-lookup"><span data-stu-id="7ed58-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="7ed58-109">Configurer SPF pour empêcher l’usurpation</span><span class="sxs-lookup"><span data-stu-id="7ed58-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
