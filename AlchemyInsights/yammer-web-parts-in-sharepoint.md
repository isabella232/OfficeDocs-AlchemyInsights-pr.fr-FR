---
title: Composants WebPart Yammer dans SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: 6868d7cdbbcc7d73e7e65fa0b0c954b4cba619ff
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157299"
---
# <a name="yammer-web-parts-in-sharepoint"></a>Composants WebPart Yammer dans SharePoint

Les composants WebPart Conversations Yammer et Points forts Yammer améliorent la collaboration sur les pages SharePoint modernes et classiques. Pour plus d’informations, voir [Conversations Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  et [points forts de Yammer](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).    

Le composant WebPart Conversations Yammer moderne est mis à jour vers la nouvelle expérience Yammer et est disponible pour les clients ciblés pour la publication. Le déploiement GA a commencé. Les nouvelles fonctionnalités incluent la possibilité de commencer une conversation avec n’importe quel billet (questions, sondages, compliments) et de marquer les réponses les plus directes directement à partir de SharePoint. Pour plus d’informations, voir [Nouveau Yammer – Conditions d’utilisation et foire aux questions](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).

 Pour identifier les composants WebPart et la configuration qui vous sont appropriés, voir [Utiliser un composant WebPart Yammer dans SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).  

**Utilisation des composants WebPart avec SharePoint Server**  

Les composants WebPart peuvent être utilisés dans des pages modernes et classiques au sein d’environnements locaux.

- Pour plus d’informations sur les pages modernes, voir [Ajouter un flux Yammer à une page moderne dans SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019). 
- Pour plus d’informations sur les pages modernes, voir [Ajouter un flux Yammer à une page moderne dans SharePoint Server 2013, 2016 et 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).

**Yammer Embed**  

Utilisez l’outil de configuration Embed pour tester l’utilisation de Embed. Une prochaine mise à jour de Embed permettra la nouvelle expérience Yammer. Pour plus d’informations, voir l’[outil de configuration de Yammer Embed](https://aka.ms/YammerEmbedConfigureTool). Pour mieux comprendre le composant de Yammer Embed, voir [Flux Embed](https://aka.ms/YammerDevDocs).

**Problèmes connus et limitations**

- Les ID de groupe ne sont pas disponibles dans les nouvelles URL Yammer qui ont été modifiées. Revenez en mode classique pour obtenir les ID de groupe ou d’autres ID d’URL.
- Les domaines personnalisés (vanity) ne sont pas pris en charge.
- Yammer Embed n’est pas optimisé pour les appareils mobiles. Utilisez les pages modernes avec le composant WebPart Yammer Conversations pour une expérience optimale.
- Les thèmes personnalisés peuvent affecter l’apparence et la facilité d’utilisation du composant WebPart Conversations sur Yammer. Ouvrez un cas de support pour signaler des problèmes.