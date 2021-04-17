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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833001"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Résolution du message des applications Microsoft 365 « Le module de plateforme de confiance de votre ordinateur ne fonctionne pas correctement »

Pour corriger cette erreur, procédez comme suit :

- Installez les dernières mises à jour [pour Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.<br/>
    **Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Essayez le processus [de récupération des utilisateurs](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) pour corriger les échecs du module de plateforme fiable (TPM).
- Définissez EnableADAL = 0 en suivant les étapes suivantes :  
    1. Cliquez avec le bouton droit sur le bouton Démarrer de Windows, choisissez **Exécuter,** tapez **regedit,** puis cliquez sur **OK.**
    2. Sélectionnez **Oui** pour autoriser l'Éditeur du Registre à apporter des modifications à votre appareil.
    3. Dans l'Éditeur du Registre, ajoutez la valeur DWORD **EnableADAL** avec le paramètre **0** sous HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pour plus d'informations, voir Problèmes de connexion lors de la connexion après la mise à jour vers [Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).