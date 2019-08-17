---
title: Les stratégies de rétention dans le centre d’administration Exchange ne fonctionnent pas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444806"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Stratégies de rétention dans le centre d’administration Exchange

 **Problème:** Les stratégies de rétention nouvellement créées ou mises à jour dans le centre d’administration Exchange ne s’appliquent pas aux boîtes aux lettres ou les éléments ne sont pas déplacés vers la boîte aux lettres d’archivage ni supprimés. 
  
 **Causes racines:**
  
- Cela peut être dû au fait que l' **Assistant dossier géré** n’a pas traité la boîte aux lettres de l’utilisateur. L’Assistant dossier géré tente de traiter toutes les boîtes aux lettres de votre organisation en nuage une fois tous les sept jours. Si vous modifiez une balise de rétention ou appliquez une autre stratégie de rétention à une boîte aux lettres, vous pouvez attendre que le dossier géré facilite le traitement de la boîte aux lettres ou exécuter l’applet de commande Start-ManagedFolderAssistant pour démarrer l’Assistant dossier géré afin de traiter un lettres. L’exécution de cette applet de commande est utile pour tester ou résoudre les problèmes d’une stratégie de rétention ou des paramètres de balise. Pour plus d’informations, consultez [la portion exécuter l’Assistant dossier géré](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Solution:** Exécutez la commande suivante pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Cela peut également se produire si **RetentionHold** a été **activé** sur la boîte aux lettres. Si la boîte aux lettres a été placée sur un RetentionHold, la stratégie de rétention de la boîte aux lettres ne sera pas traitée pendant cette période. Pour plus d’informations sur le paramètre RetentionHold, voir: conservation de rétention de [boîte aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Elle**
    
  - Vérifiez l’état du paramètre RetentionHold sur la boîte aux lettres spécifique dans [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Exécutez la commande suivante pour **Désactiver** RetentionHold sur une boîte aux lettres spécifique:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - À présent, réexécutez l’Assistant dossier géré:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Remarque:** Si la taille d’une boîte aux lettres est inférieure à 10 Mo, l’Assistant dossier géré ne traitera pas automatiquement la boîte aux lettres.
 
Pour plus d’informations sur les stratégies de rétention dans le centre d’administration Exchange, voir:
- [Balises et stratégies de rétention](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Appliquer une stratégie de rétention aux boîtes aux lettres](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Ajouter ou supprimer des balises de rétention](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Comment identifier le type de conservation placé sur une boîte aux lettres](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
