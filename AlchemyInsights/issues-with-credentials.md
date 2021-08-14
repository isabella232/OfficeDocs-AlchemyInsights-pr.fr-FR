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
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986817"
---
# <a name="issues-with-credentials"></a>Problèmes avec les informations d’identification

Plateforme d’identités Microsoft et le flux d’informations d’identification du [client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) décrivent comment programmer directement sur le flux d’octroi d’informations d’identification du client OAuth 2.0.

**Comment gérer le mot de passe ou les informations d’identification de certificat d’une application ?**

Dans l’CLI Azure, vous pouvez utiliser les informations d’identification de l’application [az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) pour supprimer, ré lister ou réinitialiser le mot de passe ou les informations d’identification de certificat d’une application.

**Réinitialisation des mots des utilisateurs**

Les utilisateurs doivent [s’inscrire à la réinitialisation du](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) mot de passe libre-service avant de pouvoir réinitialiser leur mot de passe. Une fois qu’un utilisateur s’est inscrit, il peut suivre les instructions de cet article pour réinitialiser son mot de passe : Réinitialiser votre mot de passe scolaire [ou scolaire.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Modification des mots de passe des utilisateurs**

Les utilisateurs peuvent suivre les étapes de cet article pour modifier leur mot de passe : [Comment modifier votre mot de passe](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Ils peuvent également gérer [les mots de passe d’application pour la vérification en deux étapes.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Mon utilisateur est en train de recevoir une erreur lors de la modification ou de la réinitialisation de son mot de passe**

Ce lien fournit des informations sur les problèmes courants qui peuvent survenir lorsqu’un utilisateur tente de réinitialiser son mot de passe : problèmes [courants et solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**J’ai un problème de réinitialisation du mot de passe d’un utilisateur**

- Assurez-vous que vous êtes autorisé à réinitialiser les mots de passe. *Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.* Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.

- Assurez-vous de bien comprendre les exigences de licence :

  - Vous devez avoir au moins une licence attribuée dans votre organisation :
    - **Utilisateurs cloud uniquement** : toute référence Office 365 (O365) payante ou Azure AD Basic
    - **Utilisateurs cloud et/ou** locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Pour en savoir plus sur les exigences en matière de licences, consultez La gestion des licences requise pour la réinitialisation du mot de passe en [libre-service Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Pour réinitialiser le mot de passe d’un utilisateur, recherchez-le dans Azure AD. Ensuite, dans le tableau de présentation de cet utilisateur, cliquez sur le bouton « réinitialiser le mot de passe ».

**Le bouton de réinitialisation du mot de passe est grisé**

Vous n’êtes pas autorisé à **réinitialiser les mots** de passe de cet utilisateur. *Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.* Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.

**Je ne vois pas le bouton réinitialiser le mot de passe.**

Vous n’êtes pas autorisé à réinitialiser les mots de passe. *Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur.* Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.

**Je ne vois pas le bouton Intégration locale dans la réinitialisation du mot de passe**

- Le lame d’intégration local apparaît uniquement dans les environnements hybrides, ce qui signifie que vous utilisez l’écriture écriture par mot de passe pour manipuler les mots de passe de l’utilisateur local.

- Vous ne voyez pas ce blade si :

  - Vous n’utilisez pas l’écriture écriture par mot de passe
  - Un problème est à l’installation/à la connectivité de l’écriture d’écriture par mot de passe
  - Il existe un problème avec votre installation/connectivité d’Azure AD Connecter
  - Pour plus d’informations sur la résolution des problèmes d’écriture par mot de passe, voir [Résoudre les problèmes d’écriture par mot de passe](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Je ne sais pas comment réinitialiser le mot de passe d’un utilisateur**

1. Connectez-vous au portail Azure en tant qu’administrateur approprié.
2. Go to the **Users and groups** blade, select All **Users**.
3. Sélectionnez un utilisateur dans la liste.
4. Pour l’utilisateur sélectionné, sélectionnez Vue d’ensemble, puis dans la barre de commandes, sélectionnez Réinitialiser **le mot de passe.** 
5. Sélectionnez le **bouton Réinitialiser** le mot de passe et suivez les instructions à l’écran.
    - Seules les réinitialisations effectuées via le **portail Azure** prise en charge l’écriture par mot de passe.

**Je réinitialise le mot de passe d’un utilisateur local à partir du portail Office 365 Admin ou de l’application mobile Office 365, mais l’utilisateur n’est toujours pas en mesure de se connecter**

L’écriture écriture par mot de passe n’est pas prise en charge dans ce portail. Réinitialisez le mot de passe de l’utilisateur dans le portail Azure.
