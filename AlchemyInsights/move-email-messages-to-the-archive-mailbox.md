---
title: Déplacer des messages électroniques vers la boîte aux lettres d’Archive
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28288821"
---
Des problèmes d’archivage des éléments à la boîte aux lettres d’Archive. Assurez-vous que vous avez effectué les étapes suivantes :
  
1. Vérifiez qu’une **Archive de boîte aux lettres** a été activé. Si ce n’est pas le cas, utilisez les étapes de [cet article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) pour activer la boîte aux lettres d’archive. 
    
2. Dans le centre d’administration Exchange, sélectionnez **Les balises de rétention** , sous **Gestion de la conformité**, créez une **balise de rétention** avec l’action **déplacer vers l’Archive** contenant **l’Âge de rétention**votre choix.
    
3. Dans le centre d’administration Exchange, sélectionnez les **Stratégies de rétention**, créer une **Stratégie de rétention** et ajouter votre balise de rétention **déplacer vers l’Archive** à cette stratégie. 
    
4. [Attribuer la stratégie de rétention](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aux boîtes aux lettres de l’utilisateur. La même stratégie s’appliqueront à **principale** et à la boîte aux lettres **d’Archive** . 
    
Boîte aux lettres de l’utilisateur doit maintenant avoir une stratégie d’archivage pour déplacer des éléments vers la boîte aux lettres d’Archive. Il peut être nécessaire de forcer la gérées dossier Compagnon (MFA) pour exécuter et appliquer les nouveaux paramètres de boîte aux lettres de l’utilisateur. Exécutez la commande suivante lors [connecté à PowerShell EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique : 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Plus d’informations sur la configuration d’une stratégie d’archivage, voir [configurer une stratégie d’archivage et de suppression des boîtes aux lettres](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

