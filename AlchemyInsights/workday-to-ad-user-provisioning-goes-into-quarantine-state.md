---
title: Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430744"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine

**Workday pour l’approvisionnement des utilisateurs AD passe en état de mise en quarantaine et aucun utilisateur n'est créé dans AD**

La tâche Workday pour l’approvisionnement des utilisateurs AD est passée à l’état de mise en quarantaine et les journaux d’audit affichent des événements d’échec de l’exportation avec le message d’erreur **Erreur :OperationsError-SvcErr : une erreur d’opération s’est produite. Aucune référence supérieure n’a été configurée pour le service de répertoire. Le service de répertoire est donc incapable d’émettre des références aux objets en dehors de cette forêt**. Cette erreur s’affiche généralement si le conteneur Active Directory OU n’est pas configuré correctement ou s’il existe des problèmes avec le Mappage d’expression utilisé pour **parentDistinguishedName**.

Recherchez des fautes de frappe dans la valeur par défaut OU for le paramètre **Nouveaux utilisateurs**. Veillez à ce que le conteneur OU spécifié existe déjà dans votre AD. Si vous utilisez **parentDistinguishedName** dans le mappage d’attribut, veillez à ce qu’il s’évalue toujours au conteneur connu dans le domaine AD. Recherchez l’événement Exportation dans les journaux d’audit pour afficher la valeur générée.

Pour d’autres détails sur la configuration de Workday pour l’approvisionnement automatique, voir [Tutoriel : Configurer Workday pour l'approvisionnement automatique d'utilisateurs](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

