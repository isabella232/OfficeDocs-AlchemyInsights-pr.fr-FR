---
title: Problème de réinitialisation du mot de passe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039964"
---
# <a name="problems-resetting-password"></a>Problèmes de réinitialisation du mot de passe

Voici quelques-uns des problèmes que vous pouvez être confrontés lors de la réinitialisation du mot de passe et des solutions possibles :

**J’ai un problème avec la réinitialisation de mot de passe non couverte dans les autres catégories**

- Assurez-vous que vous êtes autorisé à réinitialiser les mots de passe. Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur. Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.
- Assurez-vous de bien comprendre les exigences de licence :
    - Vous devez avoir au moins une licence attribuée dans votre organisation
        - Utilisateurs cloud uniquement : toute référence Office 365 (O365) payante ou Azure AD Basic
        - Utilisateurs cloud et/ou locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
        - Pour en savoir plus sur les conditions de licence, consultez l’article Licences requises pour la réinitialisation du mot de passe en [libre-service Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**J’ai des difficultés à tester la stratégie de réinitialisation de mot de passe que j’ai définie**

- La réplication des stratégies récemment appliquées peut prendre plusieurs minutes sur tous les centres de données et points de fin. La distance physique par rapport au centre de données affecte également la rapidité d’application des modifications.
- Testez avec un utilisateur final, et non un administrateur, et pilotez avec un petit groupe d’utilisateurs. Les stratégies configurées dans le portail Azure s’appliquent uniquement aux utilisateurs finaux, et non aux administrateurs. Microsoft applique une stratégie forte de réinitialisation de mot de passe à deux portails par défaut pour tout rôle d’administrateur Azure (exemple : administrateur général, administrateur du helpdesk, administrateur de mot de passe, etc.)
    - En savoir plus sur [les stratégies pour les administrateurs.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Je souhaite déployer la réinitialisation du mot de passe, mais je ne souhaite pas que mes utilisateurs enregistrent des informations de sécurité supplémentaires**

Pré-remplir les données de vos utilisateurs afin qu’ils n’en ont pas besoin ! - En tant qu’administrateur, vous pouvez définir les propriétés de téléphone et de messagerie de vos utilisateurs avant de déployer la réinitialisation du mot de passe dans votre organisation. Vous pouvez le faire à l’aide d’une API, De PowerShell ou d’Azure AD Connecter. Pour plus d’informations, voir :
- [Déploiement de la réinitialisation du mot de passe sans obliger les utilisateurs à s’inscrire](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Données utilisées par la réinitialisation du mot de passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Le bouton de réinitialisation du mot de passe est grisé**

Vous n’êtes pas autorisé à réinitialiser les mots de passe de cet utilisateur. Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur. Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.

**Je ne vois pas le bouton réinitialiser le mot de passe.**

Vous n’êtes pas autorisé à réinitialiser les mots de passe. Seuls les administrateurs globaux, de mot de passe et d’utilisateur peuvent réinitialiser les mots de passe utilisateur. Les administrateurs globaux peuvent également réinitialiser les mots de passe d’autres administrateurs privilégiés.

**Je ne vois pas le bouton Intégration locale dans la réinitialisation du mot de passe**

- Le lame d’intégration local apparaît uniquement dans les environnements hybrides, ce qui signifie que vous utilisez l’écriture écriture par mot de passe pour manipuler les mots de passe de l’utilisateur local.
- Vous ne voyez pas ce blade si :
    - Vous n’utilisez pas l’écriture écriture par mot de passe
    - Un problème est à l’installation/à la connectivité de l’écriture d’écriture par mot de passe
    - Il existe un problème avec votre installation/connectivité d’Azure AD Connecter
    - Pour plus d’informations sur la résolution des problèmes d’écriture par mot de passe, consultez la section Résoudre les problèmes d’écriture [par mot de passe](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Je ne sais pas comment réinitialiser le mot de passe d’un utilisateur**

1. Connectez-vous au portail Azure en tant qu’administrateur approprié.
1. Go to the Users and groups blade, select **All Users**.
1. Sélectionnez un utilisateur dans la liste.
1. Pour l’utilisateur sélectionné, sélectionnez **Vue** d’ensemble, puis dans la barre de commandes, cliquez sur **Réinitialiser le mot de passe.**
1. Suivez les instructions à l’écran.
    - Seules les réinitialisations effectuées via le portail Azure prise en charge l’écriture par mot de passe.

**Je réinitialise le mot de passe d’un utilisateur local à partir du portail Office 365 Admin ou de l’application mobile Office 365, mais l’utilisateur n’est toujours pas en mesure de se connecter**

L’écriture écriture par mot de passe n’est pas prise en charge dans ce portail. Réinitialisez à nouveau le mot de passe de l’utilisateur dans le portail Azure - portal.azure.com

