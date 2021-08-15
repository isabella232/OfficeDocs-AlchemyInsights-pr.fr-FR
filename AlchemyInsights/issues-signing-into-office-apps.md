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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986889"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Résolution du Microsoft 365 des applications « Le module de plateforme de confiance de votre ordinateur ne fonctionne pas correctement »

Pour corriger cette erreur, procédez comme suit :

- Installez les dernières mises à jour [pour Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Effacer les Office à l’aide](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows du gestionnaire d’informations d’identification.<br/>
    **Remarque :** Les chemins d’accès au Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Essayez le processus [de récupération utilisateur pour](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) corriger les défaillances du module de plateforme de confiance (TPM).
- Définissez EnableADAL = 0 en suivant les étapes suivantes :  
    1. Cliquez avec le bouton droit Windows bouton Démarrer, choisissez **Exécuter,** tapez **regedit,** puis cliquez sur **OK.**
    2. Sélectionnez **Oui** pour autoriser l’Éditeur du Registre à apporter des modifications à votre appareil.
    3. Dans l’Éditeur du Registre, ajoutez la valeur DWORD **EnableADAL** avec le paramètre **0** sous HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Pour plus d’informations, voir Problèmes de connexion lors de la connexion après la mise à jour vers [Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).