---
title: Problèmes de connexion aux applications Microsoft 365
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579935"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Résolution des applications Microsoft 365 "Désolé, un autre compte de votre organisation est déjà connecté".

Pour corriger cette erreur, procédez comme suit :

- Supprimez tous les comptes professionnels, à l’exception du compte affecté, à l’aide des paramètres Windows > **accès professionnel ou scolaire**.
- [Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br/>
    **Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. (Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)
- Ouvrez une application Office, puis **File**  >  **Account**  >  **déconnectez-vous**du compte de fichier. Ensuite, connectez-vous à l’aide d’un compte d’utilisateur avec une licence valide. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pour plus d’informations, reportez-vous à [la rubrique « Désolé, un autre compte de votre organisation est déjà connecté sur cet ordinateur » dans Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).