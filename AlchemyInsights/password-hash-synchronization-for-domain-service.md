---
title: Synchronisation du hachage de mot de passe pour service de domaine.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040864"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Synchronisation du hachage de mot de passe pour service de domaine.

**Si votre instance Azure AD DS vous invite à activer la synchronisation du hachage de mot de passe**

Vous êtes dans un scénario d’exécution d’un environnement hybride avec une synchronisation d’utilisateurs depuis un environnement Azure Active Directory Domain Services (AD DS) local. Ce scénario se produit malgré la synchronisation du hachage de mot de passe de l’environnement AD DS local à votre client Azure AD.

**Cause**

Ce scénario se produit, car Azure AD Connect par défaut ne synchronise pas les hachages de mot de passe hérités New Technology LAN Manager (NTLM) et Kerberos nécessaires pour Azure AD DS.

**Solution de contournement** 

Vous devez configurer Azure AD Connect pour synchroniser les hachages de mot de passe requis pour l’authentification NTLM et Kerberos.

Une fois Azure AD Connect configuré, un événement de modification de mot de passe ou de création de compte local synchronise alors également les hachages du mot de passe hérité avec Azure AD. Si vous souhaitez en savoir plus à ce sujet et sur l’activation de la synchronisation des mots de passe dans les environnements hybrides Azure AD DS, veuillez consulter [cette rubrique](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync).