---
title: Relayer le courrier via Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117981"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurer une application ou un périphérique multi-fonction pour envoyer des courriers électroniques

Pour découvrir les options et les étapes, consultez l’article [Comment configurer un appareil ou une application multifonction pour envoyer du courrier électronique à l’aide de Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Si vous avez un appareil ou une application qui a récemment cessé de fonctionner, les problèmes les plus courants sont les suivants :

- **Erreurs liées à l’authentification lors de l’utilisation de la soumission du client d’authentification SMTP** Nous avons récemment apporté des modifications relatives au fonctionnement de l’authentification SMTP. Pour plus d’informations sur la façon de résoudre les problèmes, consultez la section sur les échecs d’authentification de [Résolution de problèmes liés à des imprimantes, des scanneurs et des applications métier qui envoient du courrier à l’aide de Microsoft 365 ou Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Nous acceptons uniquement la version 1.2 de TLS lors de l’établissement d’une connexion sécurisée à Office 365** Si vous utilisez la connexion sécurisée (TLS), assurez-vous que votre appareil d’application prend en charge TLS 1.2. Pour plus d’informations, voir [Préparer l’utilisation de TLS 1.2 dans Office 365 et Office 365 Cloud de la communauté du secteur public.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)
 
Pour d’autres problèmes et solutions, consultez [Résolution de problèmes liés à des imprimantes, des scanneurs et des applications métier qui envoient du courrier à l’aide de Microsoft 365 ou Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Pour afficher les appareils concernés, accédez au [rapport de clients utilisant l’authentification SMTP](https://protection.office.com/mailflow/dashboard).

**Remarque** : Exchange Online ne prend pas en charge les scénarios de publipostage en bloc. Pour envoyer des e-mails commerciaux en bloc (par exemple, des bulletins d’informations client), vous devez utiliser des fournisseurs tiers spécialisés dans ces services.
