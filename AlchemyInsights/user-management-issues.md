---
title: Problèmes de gestion des utilisateurs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 70f8def2a0f3419a9aa6325e376ba52fc35ec48b61f39ede99d7e58cd6c6c464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971455"
---
# <a name="user-management-issues"></a>Problèmes de gestion des utilisateurs

**Qu'advient-il des utilisateurs actuellement affectés à l'application si je désactive la propriété « Affectation d’utilisateur requise » (définissez cette propriété sur Non) ?**

La désactivation **Affectation d’utilisateur requise** n’affecte PAS les utilisateurs actuellement affectés. La désactivation de cette propriété permet à tous les utilisateurs d'accéder à l'application. Tous les utilisateurs répertoriés et les utilisateurs affectés à des groupes dans l’application seront toujours valides.

- Pour limiter votre application à un ensemble spécifique d’utilisateurs, consultez - [Restreindre l’application Azure AD à un ensemble d’utilisateurs - Plateforme d’identités Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Pour affecter des utilisateurs et groupes à des applications d’entreprise dans Azure Active Directory (Azure AD), à partir du Portail Azure ou à l’aide de PowerShell, consultez [Gérer les affectations d’utilisateur pour une application dans Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- Pour déléguer des autorisations de création et de gestion d’applications, consultez [Déléguer des autorisations d’administrateur de gestion des applications - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Masquer des applications d’entreprise spécifiques aux utilisateurs** : pour masquer toutes les applications Microsoft 365 dans le panneau **Mes applications**. Les applications restent visibles dans le portail Office 365.

 1. Connectez-vous au portail Azure en tant qu’administrateur général de votre annuaire. 
 2. Sélectionner **Azure Active Directory**. 
 3. Sélectionner **Utilisateurs**. 
 4. Sélectionnez **Paramètres utilisateur**. 
 5. Sous **Applications d’entreprise**, cliquez sur **Gérer le lancement et l’affichage des applications pour les utilisateurs finaux**. 
 6. Pour **Les utilisateurs peuvent uniquement voir les applications Office 365 dans le portail Office 365**, cliquez sur **Oui**. 
 7. Cliquez sur **Enregistrer**. 
 8. Pour plus d’informations, consultez[Masquer une application d’entreprise de l’expérience des utilisateurs dans Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Si vous proposez une application SaaS (Software as a Service) à de nombreuses organisations, vous pouvez configurer votre application pour qu'elle accepte les ouvertures de session à partir de n'importe quel client Azure Active Directory (Azure AD). Cette configuration est appelée « Rendre votre application multi-client ». Les utilisateurs d’un client Azure AD peuvent se connecter à votre application après avoir accepté d’utiliser leur compte avec votre application. Pour plus d’informations, consultez [Créez des applications qui connectent les utilisateurs d'Azure AD - Plateforme d’identités Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Comment un utilisateur final peut-il accéder à l'application une fois qu'il a été affecté à l'application ?**

Chaque application du panneau d'applications d'entreprise possède un lien auquel les utilisateurs finaux peuvent accéder. Les utilisateurs peuvent également accéder à l’application via le portail **Mon application** en toute facilité.

- **Vous voulez savoir quelles applications et quels types d'applications sont utilisés par les utilisateurs ?**

Vous pouvez télécharger les rapports de inscription pour les 30 derniers jours à partir de **portal.azure.com > Azure Active Directory> Connexions > Télécharger les rapports**.

- Découvrez comment [Accorder l’autorisation d’un administrateur à l’échelle du client à une application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) et [Configurer la manière dont les utilisateurs finaux consentent aux applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Comprendre le [fonctionnement du consentement](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) et [Gérer le consentement aux applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


