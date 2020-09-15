---
title: Problèmes de connexion aux applications Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695285"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="5b781-102">Écran de connexion vierge dans les applications Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="5b781-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="5b781-103">Pour résoudre ce problème, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="5b781-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="5b781-104">Installez les dernières mises à jour pour [Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="5b781-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5b781-105">Réinitialiser les options d’Internet Explorer : accédez à **Outils**  >  **Internet options**  >  **avancées**  >  **réinitialisation des paramètres Internet Explorer** (Notez que vous perdez les paramètres personnalisés), puis essayez de vous connecter à nouveau à Office.</span><span class="sxs-lookup"><span data-stu-id="5b781-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="5b781-106">Désactivez Windows Defender application Guard (WDAG) ou un autre pare-feu ou antivirus similaire :</span><span class="sxs-lookup"><span data-stu-id="5b781-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="5b781-107">Dans le panneau de configuration, accédez à **programmes**, puis sélectionnez **activer ou désactiver les fonctionnalités Windows**.</span><span class="sxs-lookup"><span data-stu-id="5b781-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="5b781-108">Si Windows Defender application Guard est activé, essayez de le désactiver.</span><span class="sxs-lookup"><span data-stu-id="5b781-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="5b781-109">**Remarque :** Vous devrez peut-être redémarrer l’ordinateur.</span><span class="sxs-lookup"><span data-stu-id="5b781-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="5b781-110">Assurez-vous que le [plug-in AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) Microsoft. AAD. BrokerPlugin n’est pas bloqué par un programme d’application ou de pare-feu/antivirus.</span><span class="sxs-lookup"><span data-stu-id="5b781-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="5b781-111">[Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.</span><span class="sxs-lookup"><span data-stu-id="5b781-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5b781-112">**Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0.</span><span class="sxs-lookup"><span data-stu-id="5b781-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5b781-113">(Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5b781-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="5b781-114">Pour plus d’informations, consultez la rubrique [problèmes de connexion dans se connecter après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="5b781-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>