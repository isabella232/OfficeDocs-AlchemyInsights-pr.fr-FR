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
 <span data-ttu-id="2edd1-102">**Problème :** Nouvellement créé ou n’appliquent pas de stratégies de rétention mis à jour dans le centre d’administration Exchange pour les boîtes aux lettres ou les éléments ne sont pas déplacées vers la boîte aux lettres d’archive ou supprimés.</span><span class="sxs-lookup"><span data-stu-id="2edd1-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="2edd1-103">**Causes premières :**</span><span class="sxs-lookup"><span data-stu-id="2edd1-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="2edd1-p101">Cela peut être car **l’Assistant dossier géré** a traité pas de boîte aux lettres de l’utilisateur. L’Assistant dossier géré tente de traiter chaque boîte aux lettres dans votre organisation en nuage tous les sept jours. Si vous modifiez une balise de rétention ou appliquez une stratégie de rétention différentes à une boîte aux lettres, vous pouvez attendre jusqu'à ce que le dossier géré aider traite la boîte aux lettres, ou vous pouvez exécuter l’applet de commande Start-ManagedFolderAssistant pour démarrer l’Assistant dossier géré pour traiter un spécifique boîte aux lettres. Cette applet de commande en cours d’exécution est utile pour tester ou dépanner une stratégie de rétention ou paramètres de balises de rétention. Pour plus d’informations, visitez le site [d’exécuter l’Assistant dossier géré](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="2edd1-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="2edd1-109">**Solution :** Exécutez la commande suivante pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique :</span><span class="sxs-lookup"><span data-stu-id="2edd1-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="2edd1-p102">Cela peut également survenir si **RetentionHold** a été **activé** dans la boîte aux lettres. Si la boîte aux lettres a été placé sur un RetentionHold, la stratégie de rétention sur la boîte aux lettres n’est pas traitée pendant ce temps. Pour plus d’informations sur le paramètre, consultez RetentionHold : [Blocage de rétention de boîte aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="2edd1-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="2edd1-113">**Solution :**</span><span class="sxs-lookup"><span data-stu-id="2edd1-113">**Solution:**</span></span>
    
  - <span data-ttu-id="2edd1-114">Vérifier l’état du paramètre RetentionHold dans la boîte aux lettres spécifique dans [powershell EXO](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="2edd1-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="2edd1-115">Exécutez la commande suivante pour **désactiver** RetentionHold sur une boîte aux lettres spécifique :</span><span class="sxs-lookup"><span data-stu-id="2edd1-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="2edd1-116">Maintenant, réexécutez l’Assistant de dossier géré :</span><span class="sxs-lookup"><span data-stu-id="2edd1-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="2edd1-117">**Remarque :** Si une boîte aux lettres est inférieure à 10 Mo, l’Assistant dossier géré automatiquement traitera pas la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2edd1-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

