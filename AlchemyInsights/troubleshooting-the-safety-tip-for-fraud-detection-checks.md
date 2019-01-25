---
title: Résolution des problèmes d’info-bulle de sécurité pour la détection des fraudes vérifie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468795"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Résolution des problèmes d’info-bulle de sécurité pour la détection des fraudes vérifie

Si vous êtes l’obtention d’une info-bulle de sécurité qui indique « l’expéditeur a échoué vérifie la détection de loteries et peut ne pas être qui semblent être », puis l’expéditeur n’a pas pu passer les vérifications d’authentification DKIM soit SPF. La meilleure méthode pour résoudre ce problème est pour l’expéditeur autoriser eux-mêmes. Si l’expéditeur envoie à votre place, vous devez autoriser en ajoutant l’adresse IP de l’expéditeur à votre enregistrement SPF.
  
Pour plus d’informations, voir [résolution des problèmes d’info-bulle de sécurité (suspectes) rouge pour la détection des fraudes vérifie](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Voici quelques autres liens qui peuvent aider à :
  
- Comment Office 365 utilise SPF (Sender Policy Framework) pour éviter l’usurpation
    
- [Configurer SPF dans Office 365 pour empêcher l’usurpation](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

