---
title: Journaux des mots de passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960941"
---
# <a name="password-logs"></a>Journaux des mots de passe

**J’ai des problèmes pour accéder aux journaux d’audit de réinitialisation du mot de passe**

Pour résoudre les problèmes de réinitialisation des mots de passe dans les journaux d’audit, procédez comme suit :

Assurez-vous que vous êtes autorisé à afficher les journaux d’audit. 

Seuls les rôles suivants sont autorisés :
 - Administrateur général
 - Administrateur de sécurité
 - Lecteur Sécurité

**Je souhaite voir tous les événements d’audit de réinitialisation de mot de passe à partir du déploiement initial**

Jusqu’à 120 000 événements de réinitialisation/inscription de mot de passe sont stockés dans les rapports des 30 derniers jours. Cette limite maximale s’applique à l’interface utilisateur lors du téléchargement du fichier de valeurs séparées par des virgules. Un million d’événements sont disponibles via PowerShell.
Pour plus d’informations, consultez les liens suivants :

- [Réinitialisation des événements de mot de passe libre-service à partir de l’API Rapports et événements Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Comment télécharger rapidement des événements d’inscription de réinitialisation de mot de passe avec PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Je souhaite en savoir plus sur les fonctionnalités de réinitialisation de mot de passe**

Vérifiez qui s'inscrit ou réinitialise les mots de passe avec les journaux d'audit de réinitialisation des mots de passe Azure AD dans le Portail Azure sous **Utilisateurs et groupes**.
Pour plus d’informations, accédez aux liens suivants :

- [Vue d’ensemble des rapports de réinitialisation de mot de passe](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Afficher les rapports de réinitialisation de mot de passe dans le Portail Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Réinitialisation des événements de mot de passe libre-service à partir de l’API Rapports et événements Azure AD](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Comment télécharger rapidement des événements d’inscription de réinitialisation de mot de passe avec PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


