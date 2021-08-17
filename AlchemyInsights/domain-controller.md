---
title: 'Contrôleur de domaine '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: b044e69cef177c5a1ad38c2d27a297d90ba7f55e7b2e75fff2e390869241f325
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057892"
---
# <a name="domain-controller"></a>Contrôleur de domaine

**Échec de l’installation d’AAD-DS ou du déploiement**

Pour résoudre le problème d’échec d’activation ou de déploiement du service de domaine Azure AD (AAD-DS), effectuez les étapes suivantes :

1. Si vous utilisez un réseau virtuel existant, vérifiez les règles NSG qui bloquent les ports nécessaires à la synchronisation dans AAD-DS dans le portail https://aka.ms/aadds-networking.
2. Vérifiez si le message d’erreur que vous avez reçu est traité dans ce guide de dépannage disponible sur la page https://aka.ms/aadds-troubleshoot-enable.
3. Essayez de déployer les services de domaine Azure AD dans un nouveau réseau virtuel.
4. Suivez le guide de mise en service pour déployer AAD-DS : [Tutoriel pour créer des services de domaine AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Si vous n’arrivez pas à déployer les services de domaine Azure AD, voir [Résoudre les problèmes d'Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pour résoudre les erreurs courantes afin de résoudre les problèmes. 

**Impossible de désactiver AAD-DS**

L'AAD-DS ne peut pas être mis en pause. Si vous souhaitez arrêter d’utiliser votre domaine géré, il doit être supprimé.

Si vous rencontrez un problème, pour résoudre les messages d’erreur courants et pour consulter les étapes de dépannage qui vous aideront à reprendre votre travail, voir [Résolution des problèmes liés aux services de domaine Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
