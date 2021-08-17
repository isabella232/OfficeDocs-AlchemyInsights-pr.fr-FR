---
title: Créer un utilisateur
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118742"
---
# <a name="create-user"></a>Créer un utilisateur

**ANNONCE :**

- L’arrêt de la prise en charge de la signature WebView à partir de Google commence [le 4 janvier 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testez si vos applications peuvent être affectées en suivant les [instructions](https://go.microsoft.com/fwlink/?linkid=2157323) de Google sur le test de compatibilité.
- Veillez à utiliser la vue web système ou le navigateur système lors de la signature de vos utilisateurs avec des comptes Google grand public. Pour plus d'informations, voir [Questions relatives à la connexion à une ou plusieurs applications à l'aide du navigateur Chrome uniquement](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Je ne peux pas créer un nouvel utilisateur dans mon annuaire Azure AD**

1. Assurez-vous que vous êtes autorisé à créer un nouvel utilisateur standard. Seul le rôle Administrateur général ou Administrateur utilisateur dans Azure Active Directory (AD) peut créer un utilisateur standard. Si vous n'occupez pas l'un de ces rôles, demandez à un administrateur de vous ajouter à l'un de ces rôles ou de créer le nouveau compte utilisateur pour vous.
1. Assurez-vous que le nom d'utilisateur se trouve dans un domaine qui est vérifié dans votre AD azur. Si vous n'avez pas de nom de domaine personnalisé vérifié dans votre AD azur, vous pouvez utiliser votre domaine initial AD azur, qui se termine par *.onmicrosoft.com.
1. Assurez-vous que le nom d'utilisateur se trouve dans un domaine qui n'est pas fédéré à Azure AD depuis vos locaux AD. Les utilisateurs ne peuvent pas être ajoutés dans le cloud avec des noms de domaine qui sont fédérés à partir de locaux.
1. Assurez-vous qu'aucun autre utilisateur ou contact ne possède déjà le nom d'utilisateur que vous souhaitez attribuer au nouvel utilisateur. Les noms d'utilisateur doivent être uniques dans l' AD azur.
1. Voir [les rôles et les administrateurs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pour votre AD Azur.
1. Voir les [noms de domaine](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pour votre AD azur.
1. Consultez [les journaux d'audit](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pour obtenir des informations plus détaillées sur un utilisateur récemment créé ou supprimé, comme l'identité de la personne qui a effectué l'action et la date de celle-ci.
1. Pour plus d’informations sur l’ajout de nouveaux utilisateurs, voir Utiliser le portail Azure pour créer un utilisateur [dans votre Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Rôles d’administrateur Azure AD](/azure/active-directory/active-directory-assign-admin-roles): autorisations de rôle d’administrateur dans Azure Active Directory
1. Vous pouvez également [utiliser Azure AD PowerShell pour créer un utilisateur.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
