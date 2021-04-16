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
# <a name="issues-with-azure-mfa"></a>Problèmes avec Azure MFA
Vous pouvez vérifier si les utilisateurs ne peuvent pas se connecter à l'aide de l'authentification multifacteur (MFA)

1. L'utilisateur affecté peut être bloqué dans le portail Azure Active Directory. Si c'est le cas, les tentatives d'authentification pour cet utilisateur spécifique seront automatiquement refusées. [Suivez les étapes de cet article pour les débloquer.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si le déblocage de l'utilisateur n'a pas d'aide ou si l'utilisateur n'est pas bloqué, vous pouvez essayer de réinitialiser l'ation MFA pour l'utilisateur et il passe à nouveau par le processus d'inscription. [Suivez les étapes de cet article.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Si c'est la première fois que vous activez l'authentification multifacteur et que vos utilisateurs ne parviennent pas à se connecter à des clients autres que des navigateurs tels qu'Outlook, Skype, etc., la bibliothèque ADAL (Active Directory Authentication Library) n'est peut-être pas activée dans votre abonnement O365. Dans ce cas, vous devrez vous connecter à Exchange Online PowerShell et exécuter cette cmdlet :  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*