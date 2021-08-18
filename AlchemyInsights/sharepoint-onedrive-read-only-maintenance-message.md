---
title: Read-Only message de maintenance lors de la tentative d’utilisation SharePoint ou OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329446"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only message de maintenance lors de la tentative d’utilisation SharePoint ou OneDrive

Les utilisateurs peuvent recevoir un message en **lecture seule** pour maintenance lorsque vous essayez d’utiliser SharePoint ou OneDrive pour l’un des scénarios suivants. 

-   Une activité de maintenance planifiée ou active.  Recherchez-les en naviguant vers le [centre de messages.](https://portal.office.com/adminportal/home#/messagecenter)
-   Incident de service actif et de haute priorité qui peut se produire. Recherchez les avis/incidents en naviguant vers [l’état d’état du service.](https://portal.office.com/adminportal/home#/servicehealth)
-   Scénario de récupération de réparation automatique mineure qui pourrait se produire en raison d’événements inattendus sur les serveurs qui peuvent durer moins de 30 minutes environ. 
    
    Il n’existe aucun message de centre de messages ou d’état du service pour ces récupérations mineures, mais vous devriez être de retour à la normale très prochainement.

Dans très peu de cas, nous avons observé que l’un des trois scénarios répertoriés ci-dessus était la cause et que le service a été restauré, mais que le cache du navigateur des utilisateurs n’a pas été effacé.

Essayez d’effacer le cache du navigateur avant d’naviguer vers le site.

1. Dans votre Microsoft Edge, sélectionnez **Paramètres,** puis sélectionnez **Confidentialité et sécurité.**
2. Sous **Effacer la navigation,** **sélectionnez ce qu’il faut effacer.**
3. Sélectionnez **cookies et données de site web enregistrées,** puis **sélectionnez Effacer**.

**Remarque**: ces étapes peuvent différer lors de l’utilisation d’autres navigateurs tels que Mozilla Firefox ou Google Chrome.

**Remarque**: une autre option consisterait à ouvrir SharePoint site ou OneDrive dans une nouvelle fenêtre InPrivate.