---
title: Dépannage du Conseil de sécurité pour les vérifications de détection de fraude
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
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353247"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Dépannage du Conseil de sécurité pour les vérifications de détection de fraude

Si vous recevez un Conseil de sécurité indiquant «l’échec de nos vérifications de détection de fraude par l’expéditeur et peut ne pas être celui qu’il semble être», l’expéditeur n’a pas réussi à transmettre les contrôles d’authentification DKIM ou SPF. Pour résoudre ce cas, la meilleure méthode consiste à autoriser l’expéditeur à s’autoriser. Si l’expéditeur est envoyé en votre nom, vous devez l’autoriser en ajoutant l’adresse IP de l’expéditeur à votre enregistrement SPF.
  
Pour plus d’informations, reportez-vous à [la rubrique Troubleshooting the Red (suspect) Safety Tip for fraude DETECTION checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Voici quelques autres liens qui peuvent vous aider:
  
- [Comment Office 365 utilise Sender Policy Framework (SPF) pour éviter l’usurpation d’identité](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurer SPF dans Office 365 pour empêcher l’usurpation](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
