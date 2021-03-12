---
title: Résoudre les problèmes d' signature unique (SSO) transparente basée sur mot de passe
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709495"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="af460-102">Résoudre les problèmes d' signature unique (SSO) transparente basée sur mot de passe</span><span class="sxs-lookup"><span data-stu-id="af460-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="af460-103">Pour découvrir les principes de base de l’authentification unique basée sur un mot de passe, consultez l’authentification par mot de passe [avec Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="af460-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="af460-104">**Configurer l' utilisateur unique basé sur un mot de passe**</span><span class="sxs-lookup"><span data-stu-id="af460-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="af460-105">[Configurer l' sign-on unique](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) basée sur un mot de passe : cet article décrit plus en détail l’option DSO basée sur un mot de passe.</span><span class="sxs-lookup"><span data-stu-id="af460-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="af460-106">Si l’application que vous ajoutez nécessite une configuration personnalisée et que vous devez utiliser l’personnalisation unique basée sur un mot de passe, cet article est pour vous.</span><span class="sxs-lookup"><span data-stu-id="af460-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="af460-107">[Configurez l'](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) connexion unique basée sur un mot de passe pour les applications sur site : le proxy d’application prend en charge plusieurs modes d' connexion unique.</span><span class="sxs-lookup"><span data-stu-id="af460-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="af460-108">L’authentification basée sur un mot de passe est destinée aux applications qui utilisent une combinaison nom d’utilisateur/mot de passe pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="af460-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="af460-109">Lorsque vous configurez l' sign-on par mot de passe pour votre application, vos utilisateurs doivent se connecter une seule fois à l’application sur site.</span><span class="sxs-lookup"><span data-stu-id="af460-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="af460-110">Après cela, Azure Active Directory stocke les informations de connectez-vous et les fournit automatiquement à l’application lorsque vos utilisateurs y accèdent à distance.</span><span class="sxs-lookup"><span data-stu-id="af460-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="af460-111">Vous devez déjà avoir publié et testé votre application avec le proxy d’application.</span><span class="sxs-lookup"><span data-stu-id="af460-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="af460-112">Si ce n’est pas le cas, suivez les étapes de publication d’applications à l’aide du proxy d’application [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) puis poursuivez votre configuration de l’sO basée sur mot de passe pour les applications sur site.</span><span class="sxs-lookup"><span data-stu-id="af460-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="af460-113">Pour résoudre les problèmes d' ssO basée sur un mot de passe, voir Résoudre les problèmes d' [sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) unique basé sur mot de passe dans Azure AD</span><span class="sxs-lookup"><span data-stu-id="af460-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
