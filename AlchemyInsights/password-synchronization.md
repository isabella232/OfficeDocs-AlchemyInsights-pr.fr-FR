---
title: Synchronisation des mots de passe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960833"
---
# <a name="password-synchronization"></a>Synchronisation des mots de passe

**La synchronisation de hachage de mot de passe ne fonctionne pas du tout**

Voici quelques problèmes courants rencontrés par les clients lorsque la synchronisation de hachage de mot de passe ne fonctionne pas :

- Le compte Active Directory utilisé par Azure AD Connecter pour communiquer avec Active  Directory local  n’est pas autorisé à répliquer les modifications d’annuaire et répliquer les changements de répertoire Toutes les autorisations requises pour la synchronisation de mot de passe . Vous devez résoudre ce problème en accordant ces autorisations au compte Active Directory.
- La synchronisation de hachage de mot de passe est  désactivée après qu’un administrateur a modifié la méthode User Sign-In de synchronisation de mot de passe  à une autre option telle que la fédération avec **AD FS** dans l’Assistant Azure AD Connecter - Vous pouvez résoudre ce problème en réactivant la fonctionnalité de synchronisation de hachage de mot de passe dans l’Assistant Azure AD Connecter.
- Problème de connectivité avec Active Directory local. Par exemple, certains contrôleurs de domaine ne sont pas accessibles par Azure AD Connecter ou les [ports](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) requis sont bloqués par le pare-feu . Vous devez résoudre ce problème en vous assurant que la connectivité entre le serveur Azure AD Connecter et l’annuaire Active Directory local fonctionne correctement.
- Le serveur Azure AD Connecter est actuellement en mode intermédiaire, ce qui permettra au serveur de ne pas être en mesure d’utiliser les hésages de mot de passe . Pour résoudre le problème, suivez les étapes décrites dans la section Résoudre les problèmes de synchronisation des mots de passe avec [Azure AD Connecter -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Aucun mot de passe n’est synchronisé.

**La synchronisation de hachage de mot de passe ne fonctionne pas pour certains de mes utilisateurs**

1. Si vous avez remarqué que le hachage de  mot de passe n’est pas synchronisé pour un utilisateur, utilisez la tâche de dépannage dans le Connecter Azure AD pour examiner et résoudre le problème. Effectuez les tâches suivantes :

    a. [Exécuter la tâche de dépannage dans l’Assistant](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Utiliser la cmdlet de dépannage pour examiner le problème de synchronisation de hachage de mot de passe pour une utilisation spécifique](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. L’objet utilisateur Active Directory local est activé pour l’utilisateur doit modifier le mot de passe à la prochaine option **d’accès.** Lorsque cette option est activée, un mot de passe temporaire est attribué à l’utilisateur et est invité à le modifier lors de la prochaine fermeture de site. Azure AD Connecter ne synchronise pas les mots de passe temporaires avec Azure AD.

Pour résoudre le problème ci-dessus, effectuez l’une des tâches suivantes :

- Demandez à l’utilisateur de se connectez à l’application sur site (par exemple, Windows Bureau) et modifiez le mot de passe. Le nouveau mot de passe sera synchronisé avec Azure AD.
- Permettre à un administrateur de mettre à jour le mot de passe de l’utilisateur sans activer l’option L’utilisateur doit modifier le mot de passe à la prochaine **logonisation** et partager le nouveau mot de passe avec l’utilisateur.

3. L’objet Utilisateur Active Directory  local n’est pas correctement configuré pour la synchronisation d’objets ou la synchronisation de mot de passe. Pour résoudre ce problème, suivez les étapes décrites dans la résolution des problèmes de synchronisation de hachage de mot de passe avec [Azure AD Connecter synchronisation.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







