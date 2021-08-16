---
title: L’écriture écriture par mot de passe ne fonctionne pas
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
- "9004595"
- "8210"
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999742"
---
# <a name="password-writeback-is-not-working"></a>L’écriture écriture par mot de passe ne fonctionne pas

**J’ai des difficultés à configurer l’écriture écriture par mot de passe**

- L’écriture écriture par mot de passe est une fonctionnalité importante.
- Assurez-vous de bien comprendre les exigences de licence :
  - Vous devez avoir au moins une licence attribuée dans votre organisation
  - **Utilisateurs cloud uniquement** : toute référence Office 365 (O365) payante ou Azure AD Basic
  - **Utilisateurs cloud et/ou** locaux : Azure AD Premium P1 ou P2, Enterprise Mobility + Security (EMS) ou Secure Productive Enterprise (SPE)
    - Pour en savoir plus sur les conditions de licence requises, consultez La gestion des licences requise pour la réinitialisation du mot de passe [en libre-service Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Vous avez au moins un compte d’administrateur et un compte d’utilisateur test avec l’une des licences appropriées.
- Vous devez connecter azure AD Connecter au contrôleur de domaine principal Emulator pour que l’écriture de mot de passe fonctionne. Vous pouvez configurer Azure AD Connecter pour utiliser un contrôleur de  domaine principal en cliquant avec le bouton droit sur les propriétés du connecteur de synchronisation Active Directory, puis en sélectionnant configurer les **partitions** d’annuaire. À partir de là, recherchez la section **paramètres** de connexion du contrôleur de domaine et cochez la case intitulée utiliser uniquement les **contrôleurs de domaine préférés.**
  > [!NOTE]
  > Si le dc préféré n’est pas un émulateur PDC, Azure AD Connecter toujours atteindre le PDC pour l’écriture par mot de passe.
- La réinitialisation du mot de passe a été configurée et activée dans votre client. Pour plus d’informations, voir [Permettre aux utilisateurs de réinitialiser leurs mots de passe Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Assurez-vous que le compte d’administrateur utilisé pour activer l’écriture par mot de passe est un compte d’administrateur cloud (créé dans Azure AD et non dans AD local)
- Vous avez un déploiement local AD à forêts multiples exécutant Windows Server 2008 R2, Windows Server 2012 ou Windows Server 2012 R2 avec les derniers Service Packs installés
- Vous avez installé l’outil Connecter Azure AD et préparé votre environnement AD pour la synchronisation avec le cloud. Avant de tester l’écriture écriture par mot de passe, assurez-vous d’abord d’effectuer une importation complète et une synchronisation complète à partir d’AD et d’Azure AD dans Azure AD Connecter.
- Pour en savoir plus, découvrez comment faire une synchronisation complète et une [importation complète dans Azure AD Connecter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**J’ai un problème avec la connectivité d’écriture/écriture de mot de passe**

1. Télécharger et activer la dernière version [d’Azure AD Connecter](https://www.microsoft.com/download/details.aspx?id=47594)
2. Configuration du pare-feu : l’outil Connecter Azure AD (1.1.443 et supérieur) aura besoin d’un accès **HTTPS** sortant pour :
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Autoriser la persistance des connexions inactives pendant au moins 2 à 3 minutes

**J’ai toujours des problèmes avec l’écriture écriture par mot de passe**

- Si vous avez encore des difficultés, essayez de désactiver et de réactiver le service d’écriture par mot de passe dans l’outil d’écriture Connecter Azure AD
- Pour plus d’informations, voir comment désactiver [et réactiver](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) l’écriture par mot de passe
