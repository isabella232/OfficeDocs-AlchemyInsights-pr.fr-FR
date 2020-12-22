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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724152"
---
# <a name="comments-on-list-items"></a>Commentaires sur les éléments de liste

Les utilisateurs peuvent afficher tous les commentaires sur un élément de liste et filtrer entre les affichages affichant des commentaires ou des activités liées à un élément.

Les utilisateurs doivent noter les points suivants avant de pouvoir ajouter et supprimer des commentaires :

- Les commentaires suivent les paramètres d’autorisation inhérents à SharePoint.
- Les listes classiques qui ne sont pas encore conçues pour être affichées dans les interfaces utilisateur modernes, comme les listes de tâches, ne disposent pas de cette fonctionnalité de commentaire.
- La mise en commentaire sur des listes dans teams n’est pas disponible dans cette version.
- Les commentaires ne sont pas indexés par la recherche.

Les administrateurs peuvent désactiver cette fonctionnalité au niveau de l’organisation en modifiant le paramètre **CommentsOnListItemsDisabled** dans l’applet de commande **Set-SPOTenant** PowerShell.

Il n’est pas possible actuellement de désactiver les commentaires au niveau du site ou de la liste. Nous espérons que ces contrôles doivent être mis à jour plus tard au cours du premier trimestre 2021.
