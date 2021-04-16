---
title: Résolution des applications Microsoft 365 Votre compte se trouve dans un message d'état d'erreur
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812534"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Résolution de l'erreur « Votre compte est dans un mauvais état » des applications Microsoft 365

Pour corriger cette erreur, essayez les options suivantes sur l'ordinateur concerné :

- Ouvrez une application Office, sélectionnez **La signature du** compte de fichier de tous les  >    >  **comptes.** Reconnectez-vous à l’aide d’un compte d’utilisateur disposant d’une licence en cours. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.<br>
  **Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0. Par exemple, \Software\Microsoft\Office\16.0\Common\Identity\
- Si l'erreur se produit lors de la connexion à Office [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 365 à l'aide d'Office 2013, activez l'authentification moderne pour le client Office.

Pour plus d'informations, voir Comment résoudre les problèmes d'applications non-navigateur qui ne peuvent pas se connecter à [Microsoft 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

