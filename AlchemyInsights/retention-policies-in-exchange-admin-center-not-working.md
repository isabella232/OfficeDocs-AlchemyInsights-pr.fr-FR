---
title: Stratégies de rétention dans le centre d’administration Exchange ne fonctionne ne pas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6c69511f6bcdad5793cd2473a20a2d168d2ac260
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660705"
---
 **Problème :** Nouvellement créé ou n’appliquent pas de stratégies de rétention mis à jour dans le centre d’administration Exchange pour les boîtes aux lettres ou les éléments ne sont pas déplacées vers la boîte aux lettres d’archive ou supprimés. 
  
 **Causes premières :**
  
- Cela peut être car **l’Assistant dossier géré** a traité pas de boîte aux lettres de l’utilisateur. L’Assistant dossier géré tente de traiter chaque boîte aux lettres dans votre organisation en nuage tous les sept jours. Si vous modifiez une balise de rétention ou appliquez une stratégie de rétention différentes à une boîte aux lettres, vous pouvez attendre jusqu'à ce que le dossier géré aider traite la boîte aux lettres, ou vous pouvez exécuter l’applet de commande Start-ManagedFolderAssistant pour démarrer l’Assistant dossier géré pour traiter un spécifique boîte aux lettres. Cette applet de commande en cours d’exécution est utile pour tester ou dépanner une stratégie de rétention ou paramètres de balises de rétention. Pour plus d’informations, visitez le site [d’exécuter l’Assistant dossier géré](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solution :** Exécutez la commande suivante pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique : 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Cela peut également survenir si **RetentionHold** a été **activé** dans la boîte aux lettres. Si la boîte aux lettres a été placé sur un RetentionHold, la stratégie de rétention sur la boîte aux lettres n’est pas traitée pendant ce temps. Pour plus d’informations sur le paramètre, consultez RetentionHold : [Blocage de rétention de boîte aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Solution :**
    
  - Vérifier l’état du paramètre RetentionHold dans la boîte aux lettres spécifique dans [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Exécutez la commande suivante pour **désactiver** RetentionHold sur une boîte aux lettres spécifique : 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Maintenant, réexécutez l’Assistant de dossier géré :
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Remarque :** Si une boîte aux lettres est inférieure à 10 Mo, l’Assistant dossier géré automatiquement traitera pas la boîte aux lettres. 
  

