---
title: Mon application ne s’affiche pas dans gouvernance d’application
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362394"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Mon application ne s’affiche pas dans gouvernance d’application

Si votre application ne s’affiche pas dans la gouvernance des applications, vérifiez les choses suivantes :

1. Go to [Azure AD](https://aad.portal.azure.com/) and find the app ID for your application by searching for the app name in the top bar on the Overview page.

1. Accéder Graph Explorer et rechercher l’ID d’application dans votre principal de service à l’aide de cette requête et en remplaçant par l’ID d’application approprié : <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? $search= « appId: <appId> « >

1. Si aucun résultat n’est renvoyé, recherchez l’ID d’application dans l’application à l’aide de cette requête et en remplaçant par l’ID d’application approprié : <appId> < https://graph.microsoft.com/v1.0/applications? $search= « appId: <appId> « >

Si vous avez des problèmes avec la requête, consultez [Obtenir de l’aide.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Pour plus d’informations ou d’informations sur vos applications dans la gouvernance des applications, voir En savoir plus [sur la visibilité et les informations.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Pour plus d’informations sur l’affichage de vos applications, voir [Afficher vos applications.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)