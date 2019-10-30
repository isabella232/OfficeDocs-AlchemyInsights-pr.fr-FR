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
# <a name="issues-with-azure-mfa"></a>Problèmes avec Azure MFA
Il existe deux éléments à vérifier si les utilisateurs ne peuvent pas se connecter à l’aide de l’authentification multifacteur (MFA)

1. L’utilisateur affecté peut être bloqué dans le portail Azure Active Directory. Si c’est le cas, les tentatives d’authentification pour cet utilisateur spécifique seront refusées automatiquement. [Suivez les étapes décrites dans cet article pour les débloquer.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si le déblocage de l’utilisateur n’a pas d’aide ou si l’utilisateur n’est pas bloqué, vous pouvez essayer de réinitialiser l’authentification multifacteur pour l’utilisateur et ils feront de nouveau transiter le processus d’inscription. [Suivez les étapes décrites dans cet article.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

S’il s’agit de la première fois que vous avez activé l’authentification multifacteur et que vos utilisateurs ne peuvent pas se connecter à des clients qui ne sont pas des navigateurs tels qu’Outlook, Skype, etc., par exemple ADAL (bibliothèque d’authentification Active Directory) n’est pas activé sur votre abonnement O365. Dans ce cas, vous devez vous connecter à Exchange Online PowerShell et exécuter cette applet de commande :  *Set-OrganizationConfig-OAuth2ClientProfileEnabled : $true*