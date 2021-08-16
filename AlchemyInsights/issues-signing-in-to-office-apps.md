---
title: Problèmes de la signature à Microsoft 365 applications
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
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028038"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Résolution du Microsoft 365 des applications « Désolé, un autre compte de votre organisation est déjà signé »

Pour corriger cette erreur, procédez comme suit :

- Supprimez tous les comptes de travail, à l’exception du compte affecté, à l’aide de Windows Paramètres > **accès scolaire ou scolaire.**
- [Effacer les Office à l’aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows du gestionnaire d’informations d’identification.<br/>
    **Remarque :** Les chemins d’accès au Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Ouvrez un application Office, sélectionnez **Se**  >  **sortir du** compte de  >  **fichier.** Ensuite, connectez-vous à l’aide d’un compte d’utilisateur avec une licence valide. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Pour plus d’informations, voir [« Désolé,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)un autre compte de votre organisation est déjà inscrit sur cet ordinateur » dans Office .