---
title: Correction des applications Office votre compte est dans un message d’état incorrect
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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969429"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Correction des applications Office « votre compte est dans un état incorrect »

Pour corriger cette erreur, essayez les options suivantes sur l’ordinateur concerné :

- Ouvrez une application Office, puis **** > **** > **déconnectez-vous de tous les comptes**. Reconnectez-vous à l’aide d’un compte d’utilisateur avec une licence valide. Pour plus d’informations, consultez la rubrique [comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br>
  **Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. Par exemple, \Software\Microsoft\Office\16.0\Common\Identity\
- Sur l’ordinateur concerné, définissez EnableADAL = 0 en procédant comme suit :  
     1. Cliquez avec le bouton droit sur le bouton Windows et sélectionnez **exécuter**. Dans la zone **ouvrir** , tapez **regedit**, puis cliquez sur **OK**.
     2. Sélectionnez **Oui** lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.
    3. Dans l’éditeur du Registre, ajoutez une valeur DWORD de EnableADAL avec un paramètre de 0 sous HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Si l’erreur se produit lors de la connexion à Office 365 à l’aide d’Office 2013, [activez l’authentification moderne](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pour le client Office.

Pour plus d’informations, consultez [la rubrique résolution des problèmes liés aux applications non-navigateur qui ne peuvent pas se connecter à Office 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

