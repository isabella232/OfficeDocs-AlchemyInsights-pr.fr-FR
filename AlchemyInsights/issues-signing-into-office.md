---
title: Problèmes de connexion aux applications Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762996"
---
# <a name="issues-signing-in-to-office-apps"></a>Problèmes de connexion aux applications Office

Pour résoudre les problèmes de connexion avec les applications Office, procédez comme suit :

- Supprimez tous les comptes professionnels, à l’exception du compte affecté, à l’aide des paramètres Windows > **accès professionnel ou scolaire**.
- [Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br/>
    **Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. (Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)
- Ouvrez une application Office, puis**déconnectez-vous**du**compte** > de **fichier** > . Ensuite, connectez-vous à l’aide d’un compte d’utilisateur avec une licence valide. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Si les erreurs se produisent lors de la connexion à Microsoft 365 à l’aide d’Office 2013, activez l’authentification moderne pour le client Office.

Si vous souhaitez en savoir plus, consultez les articles : 
- [Vous ne pouvez pas vous connecter à Microsoft 365, Azure ou Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problèmes de connexion lors de la connexion après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [« Désolé, un autre compte de votre organisation est déjà connecté sur cet ordinateur » dans Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Résoudre les problèmes de connexion avec l’authentification moderne Office lors de l’utilisation d’ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)