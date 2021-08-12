---
title: Dépannage de la conseil de sécurité des vérifications de détection de fraude
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955964"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Dépannage de la conseil de sécurité des vérifications de détection de fraude

Si vous avez une conseil de sécurité qui indique « L’expéditeur a échoué à nos vérifications de détection de fraude et peut ne pas être qui il semble être », l’expéditeur n’a pas réussi à réussir les vérifications d’authentification DKIM ou SPF. La meilleure méthode pour résoudre ce problème consiste à autoriser l’expéditeur à s’autoriser lui-même. Si l’expéditeur envoie des messages en votre nom, vous devez les autoriser en ajoutant l’adresse IP de l’expéditeur à votre enregistrement SPF.
  
Pour [plus d’informations,](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voir Dépannage de la détection de conseil de sécurité rouge (suspect).
  
Voici d’autres liens qui peuvent vous aider :
  
- [Comment Microsoft utilise SPF (Sender Policy Framework) pour empêcher l’usurpation](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurer SPF pour empêcher l’usurpation d’identité](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
