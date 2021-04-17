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
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="847c9-102">Écran de sign-in vide dans les applications Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="847c9-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="847c9-103">Pour résoudre ce problème, essayez ce qui suit :</span><span class="sxs-lookup"><span data-stu-id="847c9-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="847c9-104">Installez les dernières mises à jour [pour Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="847c9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="847c9-105">Réinitialisez les options Internet Explorer : go to **Tools**  >  **Internet Options**  >  **Advanced** Reset Internet  >  **Explorer Settings** (notez que vous perdrez les paramètres personnalisés), puis essayez de vous ré-y inscrire.</span><span class="sxs-lookup"><span data-stu-id="847c9-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="847c9-106">Désactivez le Windows Defender Application Guard (WDAG) ou tout pare-feu ou programme antivirus similaire :</span><span class="sxs-lookup"><span data-stu-id="847c9-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="847c9-107">Dans le Panneau de contrôle, sélectionnez **Programmes,** puis sélectionnez Activer ou désactiver les **fonctionnalités Windows.**</span><span class="sxs-lookup"><span data-stu-id="847c9-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="847c9-108">Si Windows Defender Application Guard est activé, essayez de le désactiver.</span><span class="sxs-lookup"><span data-stu-id="847c9-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="847c9-109">**Remarque :** Vous devrez peut-être redémarrer l'ordinateur.</span><span class="sxs-lookup"><span data-stu-id="847c9-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="847c9-110">Assurez-vous que le plug-in Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) n'est bloqué par aucun programme d'application ou de pare-feu/antivirus.</span><span class="sxs-lookup"><span data-stu-id="847c9-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="847c9-111">[Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.</span><span class="sxs-lookup"><span data-stu-id="847c9-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="847c9-112">**Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0.</span><span class="sxs-lookup"><span data-stu-id="847c9-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="847c9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="847c9-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="847c9-114">Pour plus d'informations, voir Problèmes de connexion lors de la connexion après la mise à jour vers [Office 2016 build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="847c9-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>