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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088034"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Écran de sign-in vide dans Microsoft 365 applications

Pour résoudre ce problème, essayez ce qui suit :
- Installez les dernières mises à jour [pour Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Réinitialisez les options Internet Explorer : go to **Tools** Internet Options Advanced Reset Internet Explorer Paramètres (notez que vous perdrez les  >    >    >   paramètres personnalisés), puis essayez de vous Office à nouveau.
- Désactivez le Protection d’application Windows Defender (WDAG) ou tout pare-feu ou programme antivirus similaire :
    1. Dans le Panneau de contrôle, sélectionnez **Programmes,** puis Windows activer ou désactiver les fonctionnalités de **contrôle.**
    2. Si Protection d’application Windows Defender est activé, essayez de le désactiver.<br/>
    **Remarque :** Vous devrez peut-être redémarrer l’ordinateur.
- Assurez-vous que le plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) n’est bloqué par aucun programme d’application ou de pare-feu/antivirus.
- [Effacer les Office à l’aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows du gestionnaire d’informations d’identification.<br/>
    **Remarque :** Les chemins d’accès au Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Pour plus d’informations, voir Problèmes de connexion lors de la connexion après la mise à jour vers [Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).