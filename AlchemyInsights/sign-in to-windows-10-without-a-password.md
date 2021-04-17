---
title: Se connectez à Windows 10 sans utiliser de mot de passe
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830544"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="dab2c-102">Se connectez à Windows 10 sans utiliser de mot de passe</span><span class="sxs-lookup"><span data-stu-id="dab2c-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="dab2c-103">Pour éviter d'avoir à taper un mot de passe au démarrage de Windows, nous vous recommandons d'utiliser l'une des options de connectez-vous sécurisé Windows Hello, comme un code confidentiel, une reconnaissance faciale ou une empreinte digitale, si disponible.</span><span class="sxs-lookup"><span data-stu-id="dab2c-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="dab2c-104">Si vous souhaitez vraiment désactiver la sign-in sécurisée, consultez les instructions « Se connectez automatiquement à Windows 10 » ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="dab2c-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="dab2c-105">**Autres solutions Windows Hello sécurisées que le mot de passe du compte**</span><span class="sxs-lookup"><span data-stu-id="dab2c-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="dab2c-106">Go to **Settings > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="dab2c-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="dab2c-107">Les options de personnalisation disponibles sont répertoriées.</span><span class="sxs-lookup"><span data-stu-id="dab2c-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="dab2c-108">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="dab2c-108">For example:</span></span>

![Options de connectez-vous.](media/sign-in-options.png)

<span data-ttu-id="dab2c-110">Cliquez ou appuyez sur l'une des options pour la configurer.</span><span class="sxs-lookup"><span data-stu-id="dab2c-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="dab2c-111">La prochaine fois que vous démarrerez ou déverrouillez Windows, vous pourrez utiliser la nouvelle option au lieu d'un mot de passe.</span><span class="sxs-lookup"><span data-stu-id="dab2c-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="dab2c-112">**Se connectez automatiquement à Windows 10**</span><span class="sxs-lookup"><span data-stu-id="dab2c-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="dab2c-113">**Remarque**: la connectez-vous automatique est pratique, mais présente un risque de sécurité, en particulier si votre PC est accessible par plusieurs personnes.</span><span class="sxs-lookup"><span data-stu-id="dab2c-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="dab2c-114">Cliquez ou appuyez sur **le bouton** Démarrer dans la barre des tâches.</span><span class="sxs-lookup"><span data-stu-id="dab2c-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="dab2c-115">Tapez **netplwiz** et touchez la touche Entrée pour ouvrir la fenêtre Comptes d'utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="dab2c-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="dab2c-116">Dans **Comptes d'utilisateurs,** cliquez sur le compte à qui vous souhaitez vous inscrire automatiquement au démarrage de Windows.</span><span class="sxs-lookup"><span data-stu-id="dab2c-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="dab2c-117">Décochez la case « Les utilisateurs doivent entrer un nom d'utilisateur et un mot de passe pour utiliser cet ordinateur ».</span><span class="sxs-lookup"><span data-stu-id="dab2c-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Les utilisateurs doivent entrer un nom d'utilisateur et une option de mot de passe.](media/users-must-enter-username.png)

5. <span data-ttu-id="dab2c-119">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="dab2c-119">Click **OK**.</span></span> <span data-ttu-id="dab2c-120">Vous serez invité à entrer et à confirmer le mot de passe du compte que vous avez sélectionné.</span><span class="sxs-lookup"><span data-stu-id="dab2c-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="dab2c-121">Cliquez sur **OK** pour terminer.</span><span class="sxs-lookup"><span data-stu-id="dab2c-121">Click **OK** to finish.</span></span> <span data-ttu-id="dab2c-122">La prochaine fois que Windows 10 démarre, il se connecte automatiquement au compte que vous avez sélectionné.</span><span class="sxs-lookup"><span data-stu-id="dab2c-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
