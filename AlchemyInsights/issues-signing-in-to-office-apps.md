---
title: Problèmes de la signature aux applications Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833073"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Résolution du message des applications Microsoft 365 « Désolé, un autre compte de votre organisation est déjà inscrit »

Pour corriger cette erreur, procédez comme suit :

- Supprimez tous les comptes de travail, à l'exception du compte affecté, à l'aide des paramètres Windows > **accès scolaire ou scolaire.**
- [Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.<br/>
    **Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Ouvrez une application Office, sélectionnez **Se**  >  **sortir du compte** de  >  **fichier.** Ensuite, connectez-vous à l'aide d'un compte d'utilisateur avec une licence valide. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pour plus d'informations, voir « Désolé, un autre compte de votre organisation est déjà inscrit sur cet ordinateur [» dans Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)