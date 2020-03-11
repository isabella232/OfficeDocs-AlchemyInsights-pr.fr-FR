---
title: Connexion à Windows 10 sans utiliser de mot de passe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588279"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="81d6a-102">Connexion à Windows 10 sans utiliser de mot de passe</span><span class="sxs-lookup"><span data-stu-id="81d6a-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="81d6a-103">Pour éviter d’avoir à taper un mot de passe au démarrage de Windows, nous vous recommandons d’utiliser l’une des options de connexion sécurisée Windows Hello, comme un code confidentiel, une reconnaissance de visage ou une empreinte digitale, si disponible.</span><span class="sxs-lookup"><span data-stu-id="81d6a-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="81d6a-104">Si vous voulez vraiment désactiver la connexion sécurisée, consultez les instructions « connexion automatique à Windows 10 » ci-dessous.</span><span class="sxs-lookup"><span data-stu-id="81d6a-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="81d6a-105">**Solutions Windows Hello alternatives sécurisées au mot de passe du compte**</span><span class="sxs-lookup"><span data-stu-id="81d6a-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="81d6a-106">Accédez à **paramètres > comptes > options de connexion** (ou cliquez sur [ici](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="81d6a-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="81d6a-107">Les options de connexion disponibles seront affichées.</span><span class="sxs-lookup"><span data-stu-id="81d6a-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="81d6a-108">Par exemple :</span><span class="sxs-lookup"><span data-stu-id="81d6a-108">For example:</span></span>

![Options de connexion.](media/sign-in-options.png)

<span data-ttu-id="81d6a-110">Cliquez ou appuyez sur l’une des options pour la configurer.</span><span class="sxs-lookup"><span data-stu-id="81d6a-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="81d6a-111">La prochaine fois que vous démarrerez ou déverrouillerez Windows, vous serez en mesure d’utiliser la nouvelle option au lieu d’un mot de passe.</span><span class="sxs-lookup"><span data-stu-id="81d6a-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="81d6a-112">**Connexion automatique à Windows 10**</span><span class="sxs-lookup"><span data-stu-id="81d6a-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="81d6a-113">**Remarque**: la connexion automatique est pratique, mais introduit un risque de sécurité, en particulier si votre PC est accessible par plusieurs personnes.</span><span class="sxs-lookup"><span data-stu-id="81d6a-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="81d6a-114">Cliquez ou appuyez sur le bouton **Démarrer** dans la barre des tâches.</span><span class="sxs-lookup"><span data-stu-id="81d6a-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="81d6a-115">Tapez **netplwiz** et appuyez sur la touche entrée pour ouvrir la fenêtre comptes d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="81d6a-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="81d6a-116">Dans **comptes d’utilisateur**, cliquez sur le compte auquel vous souhaitez vous connecter automatiquement au démarrage de Windows.</span><span class="sxs-lookup"><span data-stu-id="81d6a-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="81d6a-117">Désactivez la case à cocher « les utilisateurs doivent entrer un nom d’utilisateur et un mot de passe pour utiliser cet ordinateur ».</span><span class="sxs-lookup"><span data-stu-id="81d6a-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Les utilisateurs doivent entrer un nom d’utilisateur et un mot de passe.](media/users-must-enter-username.png)

5. <span data-ttu-id="81d6a-119">Cliquez sur **OK**.</span><span class="sxs-lookup"><span data-stu-id="81d6a-119">Click **OK**.</span></span> <span data-ttu-id="81d6a-120">Vous serez invité à entrer et à confirmer le mot de passe du compte que vous avez sélectionné.</span><span class="sxs-lookup"><span data-stu-id="81d6a-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="81d6a-121">Cliquez sur **OK** pour terminer.</span><span class="sxs-lookup"><span data-stu-id="81d6a-121">Click **OK** to finish.</span></span> <span data-ttu-id="81d6a-122">La prochaine fois que Windows 10 démarre, il se connecte automatiquement au compte que vous avez sélectionné.</span><span class="sxs-lookup"><span data-stu-id="81d6a-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
