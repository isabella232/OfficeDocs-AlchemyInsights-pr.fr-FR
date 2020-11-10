---
title: Commentaires sur les éléments de liste
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947487"
---
# <a name="comments-on-list-items"></a>Commentaires sur les éléments de liste

Les utilisateurs seront rapidement en mesure d’ajouter et de supprimer des commentaires sur les éléments de liste. Les utilisateurs peuvent afficher tous les commentaires sur un élément de liste et filtrer entre les affichages affichant des commentaires ou des activités liées à un élément.

**Minutage** :

**Publication ciblée** : déploiement progressif à mi-octobre et attendu à mi-novembre

**Version standard** : déploiement graduel en milieu de novembre et attendu au début du 1er décembre

**Déploiement** : version ciblée pour l’ensemble de l’Organisation

Les utilisateurs doivent noter les points suivants avant de pouvoir ajouter et supprimer des commentaires :

- Les commentaires suivent les paramètres d’autorisation inhérents à SharePoint.
- Les listes classiques qui ne sont pas encore conçues pour être affichées dans les interfaces utilisateur modernes, comme les listes de tâches, ne disposent pas de cette fonctionnalité de commentaire.
- La mise en commentaire sur des listes dans teams n’est pas disponible dans cette version.
- Les commentaires ne sont pas indexés par la recherche.

Les administrateurs peuvent désactiver cette fonctionnalité au niveau de l’organisation en modifiant le paramètre **CommentsOnListItemsDisabled** dans l’applet de commande **Set-SPOTenant** PowerShell.

Il n’est pas possible actuellement de désactiver les commentaires au niveau du site ou de la liste. Nous espérons que ces contrôles doivent être mis à jour plus tard au cours du premier trimestre 2021.
