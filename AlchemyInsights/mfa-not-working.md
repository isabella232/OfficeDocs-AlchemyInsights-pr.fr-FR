---
title: Problèmes liés à l’authentification multifacteur
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768835"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cb223-102">Problèmes avec Azure MFA</span><span class="sxs-lookup"><span data-stu-id="cb223-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cb223-103">Il existe deux éléments à vérifier si les utilisateurs ne peuvent pas se connecter à l’aide de l’authentification multifacteur (MFA)</span><span class="sxs-lookup"><span data-stu-id="cb223-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cb223-104">L’utilisateur affecté peut être bloqué dans le portail Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cb223-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cb223-105">Si c’est le cas, les tentatives d’authentification pour cet utilisateur spécifique seront refusées automatiquement.</span><span class="sxs-lookup"><span data-stu-id="cb223-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cb223-106">Suivez les étapes décrites dans cet article pour les débloquer.</span><span class="sxs-lookup"><span data-stu-id="cb223-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cb223-107">Si le déblocage de l’utilisateur n’a pas d’aide ou si l’utilisateur n’est pas bloqué, vous pouvez essayer de réinitialiser l’authentification multifacteur pour l’utilisateur et ils feront de nouveau transiter le processus d’inscription.</span><span class="sxs-lookup"><span data-stu-id="cb223-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cb223-108">Suivez les étapes décrites dans cet article.</span><span class="sxs-lookup"><span data-stu-id="cb223-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cb223-109">S’il s’agit de la première fois que vous avez activé l’authentification multifacteur et que vos utilisateurs ne peuvent pas se connecter à des clients qui ne sont pas des navigateurs tels qu’Outlook, Skype, etc., par exemple ADAL (bibliothèque d’authentification Active Directory) n’est pas activé sur votre abonnement O365.</span><span class="sxs-lookup"><span data-stu-id="cb223-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cb223-110">Dans ce cas, vous devez vous connecter à Exchange Online PowerShell et exécuter cette applet de commande :  *Set-OrganizationConfig-OAuth2ClientProfileEnabled : $true*</span><span class="sxs-lookup"><span data-stu-id="cb223-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>