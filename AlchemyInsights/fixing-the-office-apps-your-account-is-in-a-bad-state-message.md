---
title: Correction des applications Office votre compte est dans un message d’état incorrect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969429"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="86acb-102">Correction des applications Office « votre compte est dans un état incorrect »</span><span class="sxs-lookup"><span data-stu-id="86acb-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="86acb-103">Pour corriger cette erreur, essayez les options suivantes sur l’ordinateur concerné :</span><span class="sxs-lookup"><span data-stu-id="86acb-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="86acb-104">Ouvrez une application Office, puis \*\*\*\* > \*\*\*\* > **déconnectez-vous de tous les comptes**.</span><span class="sxs-lookup"><span data-stu-id="86acb-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="86acb-105">Reconnectez-vous à l’aide d’un compte d’utilisateur avec une licence valide.</span><span class="sxs-lookup"><span data-stu-id="86acb-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="86acb-106">Pour plus d’informations, consultez la rubrique [comptes dans Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="86acb-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="86acb-107">[Effacez les informations d’identification Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) à l’aide du gestionnaire d’informations d’identification Windows.</span><span class="sxs-lookup"><span data-stu-id="86acb-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="86acb-108">**Remarque :** Les chemins d’accès au registre pour Office 2016 ont été modifiés en 16,0.</span><span class="sxs-lookup"><span data-stu-id="86acb-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="86acb-109">Par exemple, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="86acb-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="86acb-110">Sur l’ordinateur concerné, définissez EnableADAL = 0 en procédant comme suit :</span><span class="sxs-lookup"><span data-stu-id="86acb-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="86acb-111">Cliquez avec le bouton droit sur le bouton Windows et sélectionnez **exécuter**.</span><span class="sxs-lookup"><span data-stu-id="86acb-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="86acb-112">Dans la zone **ouvrir** , tapez **regedit**, puis cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="86acb-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="86acb-113">Sélectionnez **Oui** lorsque vous êtes invité à autoriser l’éditeur du Registre à effectuer des modifications sur votre appareil.</span><span class="sxs-lookup"><span data-stu-id="86acb-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="86acb-114">Dans l’éditeur du Registre, ajoutez une valeur DWORD de EnableADAL avec un paramètre de 0 sous HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="86acb-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="86acb-115">Si l’erreur se produit lors de la connexion à Office 365 à l’aide d’Office 2013, [activez l’authentification moderne](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pour le client Office.</span><span class="sxs-lookup"><span data-stu-id="86acb-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="86acb-116">Pour plus d’informations, consultez [la rubrique résolution des problèmes liés aux applications non-navigateur qui ne peuvent pas se connecter à Office 365, Azure ou Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="86acb-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

