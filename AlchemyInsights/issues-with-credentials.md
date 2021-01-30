---
title: Problèmes avec les informations d’identification
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052947"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="69de1-102">Problèmes avec les informations d’identification</span><span class="sxs-lookup"><span data-stu-id="69de1-102">Issues with credentials</span></span>

<span data-ttu-id="69de1-103">La plateforme d’identité Microsoft et le flux d’informations d’identification du [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) décrivent comment programmer directement sur le flux d’octroi d’informations d’identification du client OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="69de1-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="69de1-104">**Comment gérer le mot de passe ou les informations d’identification de certificat d’une application ?**</span><span class="sxs-lookup"><span data-stu-id="69de1-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="69de1-105">Dans l’CLI Azure, vous pouvez utiliser les informations d’identification de l’application [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) pour supprimer, ré lister ou réinitialiser le mot de passe ou les informations d’identification de certificat d’une application.</span><span class="sxs-lookup"><span data-stu-id="69de1-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="69de1-106">**Comment mes utilisateurs réinitialise-t-ils leur mot de passe ?**</span><span class="sxs-lookup"><span data-stu-id="69de1-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="69de1-107">Les utilisateurs doivent [s’inscrire à la réinitialisation du](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mot de passe libre-service avant de pouvoir réinitialiser leur mot de passe.</span><span class="sxs-lookup"><span data-stu-id="69de1-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="69de1-108">Une fois qu’un utilisateur s’est inscrit, il peut suivre les instructions de cet article pour réinitialiser son mot de passe : Réinitialiser votre mot de passe scolaire [ou scolaire.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="69de1-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="69de1-109">**Comment mes utilisateurs modifient-ils leur mot de passe ?**</span><span class="sxs-lookup"><span data-stu-id="69de1-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="69de1-110">Les utilisateurs peuvent suivre les étapes de cet article pour modifier leur mot de passe : [Comment modifier votre mot de passe](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="69de1-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="69de1-111">Ils peuvent également gérer [les mots de passe d’application pour la vérification en deux étapes.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="69de1-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="69de1-112">**Mon utilisateur est en train de recevoir une erreur lors de la modification ou de la réinitialisation de son mot de passe**</span><span class="sxs-lookup"><span data-stu-id="69de1-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="69de1-113">Ce lien fournit des informations sur les problèmes courants qui peuvent survenir lorsqu’un utilisateur tente de réinitialiser son mot de passe : problèmes [courants et solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="69de1-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="69de1-114">**J’ai un problème de réinitialisation du mot de passe d’un utilisateur**</span><span class="sxs-lookup"><span data-stu-id="69de1-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="69de1-115">Assurez-vous que vous êtes autorisé à réinitialiser les mots de passe.</span><span class="sxs-lookup"><span data-stu-id="69de1-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="69de1-116">*Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.*</span><span class="sxs-lookup"><span data-stu-id="69de1-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="69de1-117">Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.</span><span class="sxs-lookup"><span data-stu-id="69de1-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="69de1-118">Assurez-vous de bien comprendre les exigences de licence :</span><span class="sxs-lookup"><span data-stu-id="69de1-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="69de1-119">Vous devez avoir au moins une licence attribuée dans votre organisation :</span><span class="sxs-lookup"><span data-stu-id="69de1-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="69de1-120">**Utilisateurs cloud uniquement** : toute référence (SKU) payante Office 365 (O365) ou Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="69de1-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="69de1-121">**Utilisateurs cloud et/ou** locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="69de1-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="69de1-122">Pour en savoir plus sur les exigences en matière de licences, consultez La gestion des licences requise pour la réinitialisation du mot de passe en [libre-service Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="69de1-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="69de1-123">Pour réinitialiser le mot de passe d’un utilisateur, recherchez-le dans Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69de1-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="69de1-124">Ensuite, dans le tableau de présentation de cet utilisateur, cliquez sur le bouton « réinitialiser le mot de passe ».</span><span class="sxs-lookup"><span data-stu-id="69de1-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="69de1-125">**Le bouton de réinitialisation du mot de passe est grisé**</span><span class="sxs-lookup"><span data-stu-id="69de1-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="69de1-126">Vous n’êtes pas autorisé à **réinitialiser les mots** de passe de cet utilisateur.</span><span class="sxs-lookup"><span data-stu-id="69de1-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="69de1-127">*Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.*</span><span class="sxs-lookup"><span data-stu-id="69de1-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="69de1-128">Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.</span><span class="sxs-lookup"><span data-stu-id="69de1-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="69de1-129">**Je ne vois pas le bouton réinitialiser le mot de passe.**</span><span class="sxs-lookup"><span data-stu-id="69de1-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="69de1-130">Vous n’êtes pas autorisé à réinitialiser les mots de passe.</span><span class="sxs-lookup"><span data-stu-id="69de1-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="69de1-131">*Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.*</span><span class="sxs-lookup"><span data-stu-id="69de1-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="69de1-132">Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.</span><span class="sxs-lookup"><span data-stu-id="69de1-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="69de1-133">**Je ne vois pas le bouton Intégration locale dans la réinitialisation du mot de passe**</span><span class="sxs-lookup"><span data-stu-id="69de1-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="69de1-134">Le lame d’intégration local apparaît uniquement dans les environnements hybrides, ce qui signifie que vous utilisez l’écriture écriture par mot de passe pour manipuler les mots de passe de l’utilisateur local.</span><span class="sxs-lookup"><span data-stu-id="69de1-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="69de1-135">Vous ne voyez pas ce blade si :</span><span class="sxs-lookup"><span data-stu-id="69de1-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="69de1-136">Vous n’utilisez pas l’écriture écriture par mot de passe</span><span class="sxs-lookup"><span data-stu-id="69de1-136">You are not using password writeback</span></span>
  - <span data-ttu-id="69de1-137">Un problème est à l’installation/à la connectivité de l’écriture d’écriture par mot de passe</span><span class="sxs-lookup"><span data-stu-id="69de1-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="69de1-138">Il y a un problème avec votre installation/connectivité d’Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="69de1-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="69de1-139">Pour plus d’informations sur la résolution des problèmes d’écriture par mot de passe, voir [Résoudre les problèmes d’écriture par mot de passe](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="69de1-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="69de1-140">**Je ne sais pas comment réinitialiser le mot de passe d’un utilisateur**</span><span class="sxs-lookup"><span data-stu-id="69de1-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="69de1-141">Connectez-vous au portail Azure en tant qu’administrateur approprié.</span><span class="sxs-lookup"><span data-stu-id="69de1-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="69de1-142">Go to the **Users and groups** blade, select All **Users**.</span><span class="sxs-lookup"><span data-stu-id="69de1-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="69de1-143">Sélectionnez un utilisateur dans la liste.</span><span class="sxs-lookup"><span data-stu-id="69de1-143">Select a user from the list.</span></span>
4. <span data-ttu-id="69de1-144">Pour l’utilisateur sélectionné, sélectionnez Vue d’ensemble, puis dans la barre de commandes, sélectionnez Réinitialiser **le mot de passe.** </span><span class="sxs-lookup"><span data-stu-id="69de1-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="69de1-145">Sélectionnez le **bouton Réinitialiser** le mot de passe et suivez les instructions à l’écran.</span><span class="sxs-lookup"><span data-stu-id="69de1-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="69de1-146">Seules les réinitialisations effectuées via le **portail Azure** prise en charge l’écriture par mot de passe.</span><span class="sxs-lookup"><span data-stu-id="69de1-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="69de1-147">**Je réinitialise le mot de passe d’un utilisateur local à partir du portail d’administration Office 365 ou de l’application mobile Office 365, mais l’utilisateur n’est toujours pas en mesure de se connecter**</span><span class="sxs-lookup"><span data-stu-id="69de1-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="69de1-148">L’écriture écriture par mot de passe n’est pas prise en charge dans ce portail.</span><span class="sxs-lookup"><span data-stu-id="69de1-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="69de1-149">Réinitialisez le mot de passe de l’utilisateur dans le portail Azure.</span><span class="sxs-lookup"><span data-stu-id="69de1-149">Reset the user's password again in the Azure portal.</span></span>
