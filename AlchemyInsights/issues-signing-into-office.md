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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938206"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="47a7d-102">Problèmes de connexion aux applications Office</span><span class="sxs-lookup"><span data-stu-id="47a7d-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="47a7d-103">Pour résoudre les problèmes de connexion avec les applications Office, procédez comme suit:</span><span class="sxs-lookup"><span data-stu-id="47a7d-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="47a7d-104">Supprimez tous les comptes professionnels, à l’exception du compte affecté, à l’aide des paramètres Windows > **accès professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="47a7d-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="47a7d-105">[Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.</span><span class="sxs-lookup"><span data-stu-id="47a7d-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="47a7d-106">**Remarque:** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0.</span><span class="sxs-lookup"><span data-stu-id="47a7d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="47a7d-107">(Par exemple: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="47a7d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="47a7d-108">Ouvrez une application Office, puis déconnectez-**vous**du**compte** > de **fichier** > . Ensuite, connectez-vous à l’aide d’un compte d’utilisateur avec une licence valide.</span><span class="sxs-lookup"><span data-stu-id="47a7d-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="47a7d-109">Pour plus d’informations, consultez la rubrique [comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="47a7d-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="47a7d-110">Pour Mac, consultez la rubrique [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="47a7d-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="47a7d-111">Si les erreurs se produisent lors de la connexion à Office 365 à l’aide d’Office 2013, activez l’authentification moderne pour le client Office.</span><span class="sxs-lookup"><span data-stu-id="47a7d-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="47a7d-112">Pour plus d’informations, reportez-vous aux rubriques suivantes :</span><span class="sxs-lookup"><span data-stu-id="47a7d-112">For more information, see:</span></span>
- [<span data-ttu-id="47a7d-113">Vous ne pouvez pas vous connecter à Office 365, Azure ou Intune</span><span class="sxs-lookup"><span data-stu-id="47a7d-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="47a7d-114">Problèmes de connexion lors de la connexion après la mise à jour vers Office 2016 Build 16.0.7967 sur Windows 10</span><span class="sxs-lookup"><span data-stu-id="47a7d-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="47a7d-115">«Désolé, un autre compte de votre organisation est déjà connecté sur cet ordinateur» dans Office</span><span class="sxs-lookup"><span data-stu-id="47a7d-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="47a7d-116">Résoudre les problèmes de connexion avec l’authentification moderne Office lors de l’utilisation d’ADFS</span><span class="sxs-lookup"><span data-stu-id="47a7d-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)