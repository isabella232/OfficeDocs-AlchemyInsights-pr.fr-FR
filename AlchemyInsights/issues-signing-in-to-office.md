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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938207"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Écran de connexion vierge dans les applications Office

Pour résoudre ce problème, procédez comme suit:
- Installez les dernières mises à jour pour [Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Réinitialiser les options d’Internet Explorer: accédez à **Outils** > **Internet options** > **avancées** > réinitialisation des**paramètres Internet Explorer** (Notez que vous perdez les paramètres personnalisés), puis essayez de vous connecter à nouveau à Office.
- Désactivez Windows Defender application Guard (WDAG) ou un autre pare-feu ou antivirus similaire:
    1. Dans le panneau de configuration, accédez à **programmes**, puis sélectionnez **activer ou désactiver les fonctionnalités Windows**.
    2. Si Windows Defender application Guard est activé, essayez de le désactiver.<br/>
    **Remarque:** Vous devrez peut-être redémarrer l’ordinateur.
- Assurez-vous que le [plug-in AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BrokerPlugin n’est pas bloqué par un programme d’application ou de pare-feu/antivirus.
- [Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.<br/>
    **Remarque:** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0. (Par exemple: \Software\Microsoft\Office\16.0\Common\Identity\)

Pour plus d’informations, consultez la rubrique [problèmes de connexion dans se connecter après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).