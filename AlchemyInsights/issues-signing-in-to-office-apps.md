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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833073"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="3ffdb-102">Résolution du message des applications Microsoft 365 « Désolé, un autre compte de votre organisation est déjà inscrit »</span><span class="sxs-lookup"><span data-stu-id="3ffdb-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="3ffdb-103">Pour corriger cette erreur, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="3ffdb-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="3ffdb-104">Supprimez tous les comptes de travail, à l'exception du compte affecté, à l'aide des paramètres Windows > **accès scolaire ou scolaire.**</span><span class="sxs-lookup"><span data-stu-id="3ffdb-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="3ffdb-105">[Effacer les informations d'identification Office à l'aide](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) du Gestionnaire d'informations d'identification Windows.</span><span class="sxs-lookup"><span data-stu-id="3ffdb-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3ffdb-106">**Remarque :** Les chemins d'accès au Registre pour Office 2016 ont été modifiés en 16.0.</span><span class="sxs-lookup"><span data-stu-id="3ffdb-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3ffdb-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3ffdb-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="3ffdb-108">Ouvrez une application Office, sélectionnez **Se**  >  **sortir du compte** de  >  **fichier.** Ensuite, connectez-vous à l'aide d'un compte d'utilisateur avec une licence valide.</span><span class="sxs-lookup"><span data-stu-id="3ffdb-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="3ffdb-109">Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3ffdb-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3ffdb-110">Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="3ffdb-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="3ffdb-111">Pour plus d'informations, voir « Désolé, un autre compte de votre organisation est déjà inscrit sur cet ordinateur [» dans Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="3ffdb-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>