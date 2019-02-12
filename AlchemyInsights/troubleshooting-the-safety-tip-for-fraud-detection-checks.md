---
title: Résolution des problèmes d’info-bulle de sécurité pour la détection des fraudes vérifie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29936358"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="0bc5a-102">Résolution des problèmes d’info-bulle de sécurité pour la détection des fraudes vérifie</span><span class="sxs-lookup"><span data-stu-id="0bc5a-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="0bc5a-p101">Si vous êtes l’obtention d’une info-bulle de sécurité qui indique « l’expéditeur a échoué vérifie la détection de loteries et peut ne pas être qui semblent être », puis l’expéditeur n’a pas pu passer les vérifications d’authentification DKIM soit SPF. La meilleure méthode pour résoudre ce problème est pour l’expéditeur autoriser eux-mêmes. Si l’expéditeur envoie à votre place, vous devez autoriser en ajoutant l’adresse IP de l’expéditeur à votre enregistrement SPF.</span><span class="sxs-lookup"><span data-stu-id="0bc5a-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="0bc5a-106">Pour plus d’informations, voir [résolution des problèmes d’info-bulle de sécurité (suspectes) rouge pour la détection des fraudes vérifie](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="0bc5a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="0bc5a-107">Voici quelques autres liens qui peuvent aider à :</span><span class="sxs-lookup"><span data-stu-id="0bc5a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="0bc5a-108">Comment Office 365 utilise le contrôle sender policy framework (SPF) pour empêcher l’usurpation d’identité</span><span class="sxs-lookup"><span data-stu-id="0bc5a-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="0bc5a-109">Configurer SPF dans Office 365 pour empêcher l’usurpation</span><span class="sxs-lookup"><span data-stu-id="0bc5a-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

