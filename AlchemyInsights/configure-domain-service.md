---
title: Configurer Domain Services
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884593"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Échec de l’activation d’AAD-DS ou du déploiement

Pour résoudre le problème d’échec d’activation ou de déploiement de Azure Active Directory Domain Services (AAD-DS), procédez comme suit :

1. Si vous utilisez un réseau virtuel existant, vérifiez les règles NSG qui bloquent les ports nécessaires à la synchronisation dans AAD-DS dans le portail https://aka.ms/aadds-networking.
2. Vérifiez si le message d’erreur que vous avez reçu est traité dans ce guide de dépannage disponible sur la page https://aka.ms/aadds-troubleshoot-enable.
3. Essayez de déployer AAD-DS dans un nouveau réseau virtuel.
4. Suivez le guide de prise en main pour apprendre à déployer AAD-DS : [Créer et configurer un domaine managé Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Si vous n’arrivez pas à déployer AAD-DS, veuillez consulter la page [Erreurs courantes et étapes de dépannage pour Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) pour découvrir quelles sont les erreurs courantes et trouver comment les résoudre. 

**Impossible de désactiver AAD-DS**

AAD-DS ne peut pas être mis en pause. Si vous souhaitez arrêter d’utiliser votre domaine géré, il doit être supprimé.
Pour supprimer votre domaine géré, veuillez consulter la page [Désactiver ou supprimer un domaine managé Azure Active Directory Domain Services à partir du portail Azure](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



