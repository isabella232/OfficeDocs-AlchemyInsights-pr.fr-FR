---
title: Activer l'écriture différée de mot de passe dans Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 9dbb88492a3906f6780a345cf880327d411dcc66
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709725"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Activer l'écriture différée de mot de passe dans Azure AD Connect

Pour activer l’écriture différée de réinitialisation de mot de passe en libre-service, commencez par activer l’option d’écriture différée dans Azure AD Connect. À partir de votre serveur Azure AD Connect, procédez comme suit :

1. Connectez-vous à votre serveur Azure AD Connect et démarrez l'assistant de configuration d’**Azure AD Connect**.
2. Sur la page **Bienvenue**, cliquez sur **Configurer**.
3. Sur la page **Tâches supplémentaires**, sélectionnez **Personnaliser les options de synchronisation**, puis cliquez sur **Suivant**.
4. Sur la page **Connexion à Azure AD**, tapez vos informations d’identification d’administrateur général, puis cliquez sur Suivant.
5. Sur les pages **Connexion des annuaires** et **Filtrage par domaine/unité d'organisation**, cliquez sur**Suivant**.
6. Sur la page **Fonctionnalités facultatives**, sélectionnez **Écriture différée de mot de passe** et cliquez sur **Suivant**.
7. Sur la page**Prêt à configurer**, cliquez sur**Configurer** et attendez que le processus se termine.
8. Lorsque vous voyez que la configuration se termine, cliquez sur **Sortie**.

Avec l’écriture différée de mot de passe activée dans Azure AD Connect, configurez à présent Azure AD SSPR pour l’écriture différée.  Pour activer l’écriture différée de mot de passe dans SSPR, procédez comme suit :

1. Connectez-vous au portail Azure avec votre compte Administrateur général.
2. Recherchez et sélectionnez **Azure Active Directory**, cliquez sur **Réinitialisation du mot de passe**, puis sélectionnez **Intégration locale**.
3. Définissez l’option **Réécrire des mots de passe dans votre répertoire local ?** sur **Oui**.
4. Définissez l’option **Voulez-vous autoriser les utilisateurs à déverrouiller les comptes sans réinitialiser leur mot de passe ?** sur **Oui**.
5. Lorsque vous avez fini, cliquez sur **Enregistrer**.

Pour plus d’informations, voir [Activer l’écriture différée de réinitialisation de mot de passe en libre-service Azure Active Directory dans un environnement local](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).
