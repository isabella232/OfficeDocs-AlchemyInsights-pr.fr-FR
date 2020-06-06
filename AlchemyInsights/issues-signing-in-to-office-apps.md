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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579935"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="66447-102">Résolution des applications Microsoft 365 "Désolé, un autre compte de votre organisation est déjà connecté".</span><span class="sxs-lookup"><span data-stu-id="66447-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="66447-103">Pour corriger cette erreur, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="66447-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="66447-104">Supprimez tous les comptes professionnels, à l’exception du compte affecté, à l’aide des paramètres Windows > **accès professionnel ou scolaire**.</span><span class="sxs-lookup"><span data-stu-id="66447-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="66447-105">[Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.</span><span class="sxs-lookup"><span data-stu-id="66447-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="66447-106">**Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0.</span><span class="sxs-lookup"><span data-stu-id="66447-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="66447-107">(Par exemple : \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="66447-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="66447-108">Ouvrez une application Office, puis **File**  >  **Account**  >  **déconnectez-vous**du compte de fichier. Ensuite, connectez-vous à l’aide d’un compte d’utilisateur avec une licence valide.</span><span class="sxs-lookup"><span data-stu-id="66447-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="66447-109">Si vous souhaitez en savoir plus, consultez l’article [Les comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="66447-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="66447-110">Pour Mac, voir [Impossible de se connecter à une application Office 2016 pour Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="66447-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="66447-111">Pour plus d’informations, reportez-vous à [la rubrique « Désolé, un autre compte de votre organisation est déjà connecté sur cet ordinateur » dans Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="66447-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>