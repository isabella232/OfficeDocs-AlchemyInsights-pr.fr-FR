---
title: 2609-Retention-or-eDiscovery-Holding
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994062"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Impossible de supprimer des éléments dans SharePoint Online ou OneDrive entreprise

Vous ou vos utilisateurs pouvez ne pas être en mesure de supprimer des éléments dans SharePoint Online ou OneDrive entreprise, car une stratégie de rétention, une étiquette de rétention ou une conservation eDiscovery est appliquée à un site SharePoint ou à un élément spécifique. Il s’agit notamment de l’impossibilité de supprimer un document, une version d’un document, un dossier, une bibliothèque de documents, une liste, une application, un site ou une collection de sites. Voici quelques exemples de messages d’erreur que vous pouvez recevoir si vous essayez de supprimer un élément qui est conservé :

- « Ce site ne peut pas être supprimé, car il est inclus dans une conservation eDiscovery ou une stratégie de rétention »
- « Ce site a une stratégie de conformité définie sur bloquer la suppression »
- « Une stratégie de conformité bloque actuellement cette suppression de site »
- « Cette collection de sites ne peut pas être supprimée car elle contient des sites inclus dans une conservation eDiscovery ou une stratégie de rétention »
- « Vous devez supprimer tous les éléments de ce dossier avant de supprimer le dossier »
- « Les versions de cet élément ne peuvent pas être supprimées, car il s’agit d’une stratégie de rétention ou de conservation »
- « L’élément ne peut pas être supprimé en conservation »
- "L’étiquette appliquée à cet élément l’empêche d’être modifiée ou supprimée."
- « La liste ne peut pas être supprimée lors de la conservation ou de la stratégie de rétention »
- « La liste ne peut pas être supprimée si elle est bloquée ou si une stratégie de rétention lui est appliquée »

Pour supprimer des éléments dans l’un de ces scénarios, la stratégie de rétention, l’étiquette de rétention ou le blocage eDiscovery doit être supprimé (ou un site doit être exclu d’une stratégie de rétention). Vous devez désactiver ou exclure le blocage respectif qui est à l’origine de ce problème. Après la suppression d’une stratégie de rétention ou d’une conservation, la modification peut prendre jusqu’à 24 heures. 

Pour plus d’informations sur les différentes fonctionnalités de rétention et de conservation pouvant être appliquées aux sites SharePoint et aux comptes OneDrive, consultez l’une des rubriques suivantes.

- [Vue d’ensemble des stratégies de rétention](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Vue d’ensemble des étiquettes de rétention](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Gérer les suspensions dans Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [conservations eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Stratégies de fermeture et de suppression de site héritées](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
