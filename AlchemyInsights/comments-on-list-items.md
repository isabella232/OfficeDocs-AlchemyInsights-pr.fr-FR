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
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995485"
---
# <a name="comments-on-list-items"></a>Commentaires sur les éléments de liste

Les utilisateurs peuvent afficher tous les commentaires sur un élément de liste et filtrer entre les vues qui montrent les commentaires ou l’activité liée à un élément.

Les utilisateurs doivent noter les remarques suivantes avant de pouvoir ajouter et supprimer des commentaires :

- Les commentaires suivent les paramètres d’autorisation inhérents SharePoint.
- Les listes classiques qui ne sont pas encore conçues pour s’afficher dans les interfaces utilisateur modernes, comme les listes de tâches, n’auront pas cette fonctionnalité de commentaires.
- Les commentaires sur les listes Teams’est pas disponible avec cette version.
- Les commentaires ne sont pas indexés par la recherche.

Les administrateurs peuvent désactiver cette fonctionnalité au niveau de l’organisation en modifiant le paramètre **CommentsOnListItemsDisabled** dans la cmdlet **Set-SPOTenant** PowerShell.

Il n’est actuellement pas possible de désactiver les commentaires au niveau du site ou de la liste. Nous espérons que ces contrôles seront mis à jour ultérieurement, probablement au cours du premier trimestre 2021.
