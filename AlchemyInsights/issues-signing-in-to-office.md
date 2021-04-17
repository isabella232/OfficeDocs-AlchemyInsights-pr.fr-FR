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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833029"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Écran de sign-in vide dans les applications Microsoft 365

Pour résoudre ce problème, essayez ce qui suit :
- Installez les dernières mises à jour [pour Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Réinitialisez les options Internet Explorer : go to **Tools**  >  **Internet Options**  >  **Advanced** Reset Internet  >  **Explorer Settings** (notez que vous perdrez les paramètres personnalisés), puis essayez de vous ré-y inscrire.
- Désactivez le Windows Defender Application Guard (WDAG) ou tout pare-feu ou programme antivirus similaire :
    1. Dans le Panneau de contrôle, sélectionnez **Programmes,** puis sélectionnez Activer ou désactiver les **fonctionnalités Windows.**
    2. Si Windows Defender Application Guard est activé, essayez de le désactiver.<br/>
    **Remarque :** Vous devrez peut-être redémarrer l'ordinateur.
- Assurez-vous que le plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) n'est bloqué par aucun programme d'application ou de pare-feu/antivirus.
- [Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.<br/>
    **Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Pour plus d'informations, voir Problèmes de connexion lors de la connexion après la mise à jour vers [Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).