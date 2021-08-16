---
title: Problèmes avec l’famf
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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098600"
---
# <a name="issues-with-azure-mfa"></a>Problèmes avec Azure MFA
Vous pouvez vérifier si les utilisateurs ne peuvent pas se connecter à l’aide de l’authentification multifacteur (MFA)

1. L’utilisateur affecté peut être bloqué dans Azure Active Directory Portal. Si c’est le cas, les tentatives d’authentification pour cet utilisateur spécifique seront automatiquement refusées. [Suivez les étapes de cet article pour les débloquer.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si le déblocage de l’utilisateur n’a pas d’aide ou si l’utilisateur n’est pas bloqué, vous pouvez essayer de réinitialiser l’ation MFA pour l’utilisateur et il passe à nouveau par le processus d’inscription. [Suivez les étapes de cet article.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Si c’est la première fois que vous activez l’authentification multifacteur et que vos utilisateurs ne parviennent pas à se connecter à des clients autres que des navigateurs tels que Outlook, Skype, etc., il se peut qu’ADAL (Active Directory Authentication Library) ne soit pas activé dans votre abonnement O365. Dans ce cas, vous devez vous connecter à Exchange Online PowerShell et exécuter cette cmdlet : *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*