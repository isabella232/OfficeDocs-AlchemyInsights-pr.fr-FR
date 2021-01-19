---
title: Dépanner les problèmes des utilisateurs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886853"
---
# <a name="announcements"></a>Annonces

Suivez les conseils de Google sur les tests de compatibilité pour vérifier si vos applications sont affectées. Le guide de Google est disponible en https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.

Assurez-vous d'utiliser le système webview ou le navigateur système lorsque vous connectez à vos utilisateurs avec des comptes Google grand public. Pour plus d'informations, voir [Questions relatives à la connexion à une ou plusieurs applications à l'aide du navigateur Chrome uniquement](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Je ne peux pas créer un nouvel utilisateur dans mon annuaire Azure AD**

Pour résoudre le problème de l'impossibilité de créer un nouvel utilisateur dans Azure AD, suivez les étapes suivantes :

1. Assurez-vous que vous êtes autorisé à créer un nouvel utilisateur standard. Seul le rôle d'administrateur global ou d'administrateur des utilisateurs dans Azure Active Directory (AD) peut créer un nouvel utilisateur standard. Si vous n'occupez pas l'un de ces rôles, demandez à un administrateur de vous ajouter à l'un de ces rôles ou de créer le nouveau compte utilisateur pour vous.
2. Assurez-vous que le nom d'utilisateur se trouve dans un domaine qui est vérifié dans votre AD azur. Si vous n'avez pas de nom de domaine personnalisé vérifié dans votre AD azur, vous pouvez utiliser votre domaine initial AD azur, qui se termine par *.onmicrosoft.com.
3. Assurez-vous que le nom d'utilisateur se trouve dans un domaine qui n'est pas fédéré à Azure AD depuis vos locaux AD. Les utilisateurs ne peuvent pas être ajoutés dans le cloud avec des noms de domaine qui sont fédérés à partir de locaux.
4. Assurez-vous qu'aucun autre utilisateur ou contact ne possède déjà le nom d'utilisateur que vous souhaitez attribuer au nouvel utilisateur. Les noms d'utilisateur doivent être uniques dans l' AD azur.
5. Voir [les rôles et les administrateurs](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) pour votre AD Azur.
6. Voir les [noms de domaine](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) pour votre AD azur.
7. Consultez [les journaux d'audit](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) pour obtenir des informations plus détaillées sur un utilisateur récemment créé ou supprimé, comme l'identité de la personne qui a effectué l'action et la date de celle-ci.
8. Pour plus d'informations sur l'ajout de nouveaux utilisateurs, voir [Utiliser le portail Azure pour créer un nouvel utilisateur dans votre AD Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).
9. Pour plus d'informations sur les autorisations de rôle d'administrateur dans Azure AD, voir [les rôles administratifs dans Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Pour plus de détails sur la création d'un utilisateur utilisant Azure AD Powershell, voir[Azure AD PowerShell pour créer un nouvel utilisateur](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Problème avec l'inscription en libre-service**

Pour résoudre les problèmes liés à l'inscription en libre-service, suivez les étapes suivantes :

1. Pour utiliser l'inscription en libre-service avec vos applications, activez d'abord l'inscription en libre-service pour votre locataire. 
2. Pour permettre à une application de prendre en charge l'inscription en libre-service, ajoutez-la à votre flux d'utilisateurs . La prochaine fois que vous irez sur la page de connexion de cette application, vous verrez une option * *_Pas de compte ? Créez-en un !_* _. Cela permet de lancer le processus d'inscription en libre-service.
3. Pour savoir comment utiliser l'inscription en libre-service pour alimenter une organisation en Azure AD, voir [Inscription en libre-service pour Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Une fois que vous associez le flux d'utilisateurs à une ou plusieurs applications, les utilisateurs qui visitent cette application pourront s'inscrire et obtenir un compte d'invité en utilisant les options configurées dans le flux d'utilisateurs. Pour plus d'informations sur l'inscription et l'obtention d'un compte d'invité, les utilisateurs peuvent voir [l'inscription en libre-service pour les utilisateurs invités](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Problème d'invitation d'un utilisateur externe**

Pour résoudre les problèmes liés à l'invitation d'un utilisateur externe, effectuez l'étape suivante :

Assurez-vous que vous envoyez l'invitation d'un utilisateur à d' e-mail qui correspond au nom avec lequel l'utilisateur s'est inscrit. Si vous envoyez l'invitation à l'adresse e-mail proxy d'un utilisateur, ce dernier ne peut pas l'échanger. Pour plus d'informations, voir [la documentation B2B de Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/) .

**Je ne peux pas attribuer de licences à un utilisateur**

Pour résoudre les problèmes liés à l'attribution de licences à un utilisateur, suivez les étapes suivantes :

1. Pour gérer les licences d'utilisation, assurez-vous que vous utilisez un compte avec l'un des rôles d'administrateur requis : administrateur global, administrateur de licences ou administrateur d'utilisateurs. Vous pouvez vérifier le rôle de l'utilisateur dans l'onglet **Rôle de l'annuaire** sur la lame de l'utilisateur.
2. Si vous utilisez le portail Azure et que l'attribution des licences échoue, cliquez sur la notification dans le coin supérieur droit. Cela ouvre une lame avec des détails sur ce qui a mal tourné. Dans la plupart des cas, cela suffit pour comprendre et résoudre le problème.
3. Avant qu'une licence puisse être assignée à un utilisateur, assurez-vous que la propriété **Usage Location** est définie pour l'utilisateur. Vérifiez que l'utilisateur a bien cette propriété en consultant l'onglet **Profil** sur la lame de l'utilisateur.
4. Assurez-vous qu'il y a suffisamment de licences disponibles pour le produit que vous essayez d'assigner. Vous pouvez voir le nombre de licences disponibles dans le portail Azure, à l'adresse [ Azure Active Directory -> Licences -> Tous les produits](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. L'utilisateur peut déjà avoir une autre licence dont les services sont en conflit avec ceux de la nouvelle licence que vous essayez d'attribuer. Par exemple, si l'utilisateur a activé le service d'échange en ligne (plan 1), vous ne pourrez pas lui attribuer de licence avec l'échange en ligne (plan 2). Désactivez l'un des services pour permettre la nouvelle attribution de licence. Si vous utilisez le portail Azure ou les cmdlets PowerShell, la **page des détails** du problème énumère les services spécifiques qui sont à l'origine du conflit.
6. Si vous essayez de supprimer une licence et que cela échoue, l'utilisateur peut avoir d'autres licences avec des services qui dépendent des services que vous essayez de supprimer. Si vous utilisez le portail Azure ou les cmdlets PowerShell, le message d'erreur énumérera les services spécifiques qui ont des dépendances.
7. Si vous voulez comprendre pourquoi une licence a été ajoutée/supprimée à un utilisateur (par exemple, qui d'autre dans votre organisation peut avoir fait des changements), consultez les journaux d'audit. Définissez le filtre sur **activités de licence** pour afficher toutes les modifications, y compris l'« acteurs » qui les a effectuées.
8. Si vous utilisez Exchange Online, certains utilisateurs de votre locataire peuvent être incorrectement configurés avec la même valeur d'adresse proxy. Dans ce cas, vous pouvez voir des messages d'erreur génériques lorsqu'une opération de licence échoue. [Cet article](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contient plus d'informations sur ce problème, notamment des informations sur [comment se connecter à Exchange Online à l'aide de PowerShell à distance](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).Pour identifier les utilisateurs chez votre locataire, contenant la même adresse proxy, exécutez ce cmdlet Exchange Online :

Exécuter

Obtenir le destinataire | où {$_.EmailAddresses -match <user principal name>} | fL Nom, type de destinataire, e-mail





