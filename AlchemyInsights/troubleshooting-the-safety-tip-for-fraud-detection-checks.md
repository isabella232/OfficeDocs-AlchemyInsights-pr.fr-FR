---
title: Dépannage du conseil de sécurité pour les vérifications de détection de fraude
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834729"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Dépannage du conseil de sécurité pour les vérifications de détection de fraude

Si vous avez un conseil de sécurité qui indique « L'expéditeur a échoué à nos vérifications de détection des fraudes et n'est peut-être pas ce qu'il semble être », l'expéditeur n'a pas réussi les vérifications d'authentification DKIM ou SPF. La meilleure méthode pour résoudre ce problème consiste à autoriser l'expéditeur à s'autoriser lui-même. Si l'expéditeur envoie en votre nom, vous devez les autoriser en ajoutant l'adresse IP de l'expéditeur à votre enregistrement SPF.
  
Pour plus [d'informations,](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voir Dépannage du conseil de sécurité rouge (suspect) pour les vérifications de détection de fraude.
  
Voici d'autres liens qui peuvent vous aider :
  
- [Comment Microsoft utilise SPF (Sender Policy Framework) pour empêcher l'usurpation](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurer SPF pour empêcher l’usurpation d’identité](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
