---
title: Problèmes avec mfa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810482"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="2c4cc-102">Problèmes avec Azure MFA</span><span class="sxs-lookup"><span data-stu-id="2c4cc-102">Issues with Azure MFA</span></span>
<span data-ttu-id="2c4cc-103">Vous pouvez vérifier si les utilisateurs ne peuvent pas se connecter à l'aide de l'authentification multifacteur (MFA)</span><span class="sxs-lookup"><span data-stu-id="2c4cc-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2c4cc-104">L'utilisateur affecté peut être bloqué dans le portail Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2c4cc-105">Si c'est le cas, les tentatives d'authentification pour cet utilisateur spécifique seront automatiquement refusées.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2c4cc-106">Suivez les étapes de cet article pour les débloquer.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2c4cc-107">Si le déblocage de l'utilisateur n'a pas d'aide ou si l'utilisateur n'est pas bloqué, vous pouvez essayer de réinitialiser l'ation MFA pour l'utilisateur et il passe à nouveau par le processus d'inscription.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2c4cc-108">Suivez les étapes de cet article.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2c4cc-109">Si c'est la première fois que vous activez l'authentification multifacteur et que vos utilisateurs ne parviennent pas à se connecter à des clients autres que des navigateurs tels qu'Outlook, Skype, etc., la bibliothèque ADAL (Active Directory Authentication Library) n'est peut-être pas activée dans votre abonnement O365.</span><span class="sxs-lookup"><span data-stu-id="2c4cc-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2c4cc-110">Dans ce cas, vous devrez vous connecter à Exchange Online PowerShell et exécuter cette cmdlet :  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="2c4cc-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>