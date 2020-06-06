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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579863"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Résolution des applications Microsoft 365 les applications « le module de plateforme approuvée de votre ordinateur ne fonctionne pas correctement » s’affiche

Pour corriger cette erreur, procédez comme suit :

- Installez les dernières mises à jour pour [Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Effacez les informations d’identification Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br/>
    **Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. (Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)
- Essayez le [processus de récupération](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) par l’utilisateur pour corriger les défaillances du module de plateforme sécurisée (TPM).
- Définissez EnableADAL = 0 en procédant comme suit :  
    1. Cliquez avec le bouton droit sur le bouton Démarrer de Windows, choisissez **exécuter**, tapez **regedit**, puis cliquez sur **OK**.
    2. Sélectionnez **Oui** pour autoriser l’éditeur du Registre à modifier votre appareil.
    3. Dans l’éditeur du Registre, ajoutez une valeur DWORD de **EnableADAL** avec un paramètre de **0** sous HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Pour plus d’informations, consultez la rubrique [problèmes de connexion dans se connecter après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).