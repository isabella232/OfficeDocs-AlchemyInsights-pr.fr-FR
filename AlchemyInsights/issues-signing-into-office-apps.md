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
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="52e2d-102">Résolution des applications Microsoft 365 les applications « le module de plateforme approuvée de votre ordinateur ne fonctionne pas correctement » s’affiche</span><span class="sxs-lookup"><span data-stu-id="52e2d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="52e2d-103">Pour corriger cette erreur, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="52e2d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="52e2d-104">Installez les dernières mises à jour pour [Windows](https://support.microsoft.com/help/4027667/windows-10-update) et [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="52e2d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="52e2d-105">[Effacez les informations d’identification Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.</span><span class="sxs-lookup"><span data-stu-id="52e2d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="52e2d-106">**Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0.</span><span class="sxs-lookup"><span data-stu-id="52e2d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="52e2d-107">(Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="52e2d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="52e2d-108">Essayez le [processus de récupération](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) par l’utilisateur pour corriger les défaillances du module de plateforme sécurisée (TPM).</span><span class="sxs-lookup"><span data-stu-id="52e2d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="52e2d-109">Définissez EnableADAL = 0 en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="52e2d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="52e2d-110">Cliquez avec le bouton droit sur le bouton Démarrer de Windows, choisissez **exécuter**, tapez **regedit**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="52e2d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="52e2d-111">Sélectionnez **Oui** pour autoriser l’éditeur du Registre à modifier votre appareil.</span><span class="sxs-lookup"><span data-stu-id="52e2d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="52e2d-112">Dans l’éditeur du Registre, ajoutez une valeur DWORD de **EnableADAL** avec un paramètre de **0** sous HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="52e2d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="52e2d-113">Pour plus d’informations, consultez la rubrique [problèmes de connexion dans se connecter après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="52e2d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>