---
title: Résolution des applications Microsoft 365 votre compte présente un message d’état incorrect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 264307f23a349ef4ebf40f48ddbcddd3216a4927
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580115"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Résolution de l’erreur « état incorrect de vos applications Microsoft 365 »

Pour corriger cette erreur, essayez les options suivantes sur l’ordinateur concerné :

- Ouvrez une application Office **, puis**  >  **Account**  >  **déconnectez-vous de tous les comptes**. Reconnectez-vous à l’aide d’un compte d’utilisateur disposant d’une licence en cours. Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br>
  **Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. Par exemple, \Software\Microsoft\Office\16.0\Common\Identity\
- Si l’erreur se produit lors de la connexion à Office 365 à l’aide d’Office 2013, [activez l’authentification moderne](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pour le client Office.

Pour plus d’informations, consultez [la rubrique résolution des problèmes liés aux applications non-navigateur qui ne peuvent pas se connecter à Microsoft 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

