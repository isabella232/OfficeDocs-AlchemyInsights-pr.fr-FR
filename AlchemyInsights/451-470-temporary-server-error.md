---
title: 451 4.7.0 Erreur de serveur temporaire. Veuillez réessayer plus tard. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 16e16f087c2b13a9ad5fec7223b4f3395e42646e
ms.sourcegitcommit: 380ee556007d2be389b1a99795bca04bc1f9f60f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53604917"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Erreur de serveur temporaire. Veuillez réessayer plus tard. PRX4

Vous pouvez être confronté à un problème lors de l’envoi de messages électroniques via Smarthost « smtp.office365.com » à l’aide de la méthode d’envoi de client SMTP et recevoir l’erreur : « Erreur de serveur temporaire 451 4.7.0. Veuillez réessayer plus tard. PRX4 est principalement temporaire. » 

Assurez-vous que vous n’utilisez pas de boîte aux lettres partagée pour l’envoi de client SMTP, car la méthode d’envoi du client SMTP nécessite une boîte aux lettres sous licence pour envoyer des messages électroniques. Toutefois, si vous n’utilisez pas une boîte aux lettres partagée et que le problème persiste, vérifiez les points suivants :

1. Activez l’envoi SMTP client sur la boîte aux lettres sous licence utilisée en exécutant cette commande PowerShell :

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OU

    1. Go to the Centre d’administration Microsoft 365 > **Active users**, and select the user.
    1. Go to Mail tab > **Email apps** > select Manage **email apps**. 
    1. Assurez-vous que **le paramètre SMTP** authentifié est activé.
    1. Sélectionnez **Enregistrer les modifications**.
    
    Pour activer l’authentification SMTP pour l’ensemble d’une organisation, exécutez la commande ci-après :

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Remarque**: pour des raisons de sécurité, il est recommandé d’activer l’authentification SMTP uniquement pour la boîte aux lettres utilisée. Le paramètre au niveau de l’utilisateur remplace le paramètre au niveau de l’organisation.

2. Désactivez les paramètres par défaut de sécurité Azure en désactivant Activer les **paramètres de sécurité** par défaut sur **Non**:

    1. Connectez-vous au portail Azure en tant qu’administrateur de sécurité, administrateur d’accès conditionnel ou administrateur général.
    1. Accédez à Azure Active Directory >**  propriétés et** sélectionnez **Gérer les paramètres de sécurité par défaut.**
    1. Définissez **le basculement Activer les paramètres** de sécurité par défaut sur **Non.**
    1. Sélectionnez **Enregistrer**.

3. Désactivez l’authentification multifacteur (MFA) sur la boîte aux lettres sous licence utilisée.

    1. Go to the Centre d’administration Microsoft 365, and in the left navigation menu choose **Users**  >  **Active users**.
    1. Sur la page **Utilisateurs actifs**, sélectionnez **Authentification multifacteur**.
    1. Sélectionnez l’utilisateur et désactivez **l’authentification multifacteur.**

