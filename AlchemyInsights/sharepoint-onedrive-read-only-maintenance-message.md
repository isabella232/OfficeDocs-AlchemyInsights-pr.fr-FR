---
title: Lecture seule pour un message de maintenance lors de la tentative d’utilisation de SharePoint ou OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620721"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Lecture seule pour un message de maintenance lors de la tentative d’utilisation de SharePoint ou OneDrive

Les utilisateurs peuvent recevoir un message **de maintenance en lecture seule** lorsqu’ils tentent d’utiliser SharePoint ou OneDrive pour l’un des scénarios suivants. 

-   Activité de maintenance planifiée ou active.  Vérifiez-les en accédant au [Centre de messages](https://portal.office.com/adminportal/home#/messagecenter).
-   Un incident de service actif de haute priorité susceptible de se produire. Recherchez les avis/incidents en accédant à l' [État du service](https://portal.office.com/adminportal/home#/servicehealth).
-   Un scénario de récupération de réparation automatique mineur qui peut être dû à des événements inattendus sur les serveurs qui peuvent durer moins de 30 minutes ou plus. 
    
    Il n’existe aucune publication de centre de messages ou d’intégrité de service pour ces récupérateurs mineurs, mais vous devriez être redirigé vers la version normale très prochainement.

En très peu de occasions, nous avons observé que l’un des trois scénarios mentionnés ci-dessus était la cause, et que le service a été restauré, mais que le cache du navigateur des utilisateurs n’a pas été effacé.

Essayez de vider le cache du navigateur avant de naviguer sur le site.

1. Dans votre navigateur Microsoft Edge, sélectionnez **paramètres**, puis **confidentialité et sécurité**.
2. Sous **effacer la navigation**, sélectionnez **choisir les éléments à effacer**.
3. Sélectionnez **cookies et données de site Web enregistrées**, puis sélectionnez **Effacer**.

>[!Note] 
> Ces étapes peuvent varier en cas d’utilisation d’autres navigateurs, tels que Mozilla Firefox ou Google Chrome.

>[!Note] 
> Une autre option consiste à ouvrir votre site SharePoint ou OneDrive dans une nouvelle fenêtre InPrivate.