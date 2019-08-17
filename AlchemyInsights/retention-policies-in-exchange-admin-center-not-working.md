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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="c32d6-102">Stratégies de rétention dans le centre d’administration Exchange</span><span class="sxs-lookup"><span data-stu-id="c32d6-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="c32d6-103">**Problème:** Les stratégies de rétention nouvellement créées ou mises à jour dans le centre d’administration Exchange ne s’appliquent pas aux boîtes aux lettres ou les éléments ne sont pas déplacés vers la boîte aux lettres d’archivage ni supprimés.</span><span class="sxs-lookup"><span data-stu-id="c32d6-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="c32d6-104">**Causes racines:**</span><span class="sxs-lookup"><span data-stu-id="c32d6-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="c32d6-105">Cela peut être dû au fait que l' **Assistant dossier géré** n’a pas traité la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c32d6-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="c32d6-106">L’Assistant dossier géré tente de traiter toutes les boîtes aux lettres de votre organisation en nuage une fois tous les sept jours.</span><span class="sxs-lookup"><span data-stu-id="c32d6-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="c32d6-107">Si vous modifiez une balise de rétention ou appliquez une autre stratégie de rétention à une boîte aux lettres, vous pouvez attendre que le dossier géré facilite le traitement de la boîte aux lettres ou exécuter l’applet de commande Start-ManagedFolderAssistant pour démarrer l’Assistant dossier géré afin de traiter un lettres.</span><span class="sxs-lookup"><span data-stu-id="c32d6-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="c32d6-108">L’exécution de cette applet de commande est utile pour tester ou résoudre les problèmes d’une stratégie de rétention ou des paramètres de balise.</span><span class="sxs-lookup"><span data-stu-id="c32d6-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="c32d6-109">Pour plus d’informations, consultez [la portion exécuter l’Assistant dossier géré](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="c32d6-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="c32d6-110">**Solution:** Exécutez la commande suivante pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique:</span><span class="sxs-lookup"><span data-stu-id="c32d6-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="c32d6-111">Cela peut également se produire si **RetentionHold** a été **activé** sur la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c32d6-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="c32d6-112">Si la boîte aux lettres a été placée sur un RetentionHold, la stratégie de rétention de la boîte aux lettres ne sera pas traitée pendant cette période.</span><span class="sxs-lookup"><span data-stu-id="c32d6-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="c32d6-113">Pour plus d’informations sur le paramètre RetentionHold, voir: conservation de rétention de [boîte aux lettres](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="c32d6-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="c32d6-114">**Elle**</span><span class="sxs-lookup"><span data-stu-id="c32d6-114">**Solution:**</span></span>
    
  - <span data-ttu-id="c32d6-115">Vérifiez l’état du paramètre RetentionHold sur la boîte aux lettres spécifique dans [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="c32d6-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="c32d6-116">Exécutez la commande suivante pour **Désactiver** RetentionHold sur une boîte aux lettres spécifique:</span><span class="sxs-lookup"><span data-stu-id="c32d6-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="c32d6-117">À présent, réexécutez l’Assistant dossier géré:</span><span class="sxs-lookup"><span data-stu-id="c32d6-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="c32d6-118">**Remarque:** Si la taille d’une boîte aux lettres est inférieure à 10 Mo, l’Assistant dossier géré ne traitera pas automatiquement la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c32d6-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="c32d6-119">Pour plus d’informations sur les stratégies de rétention dans le centre d’administration Exchange, voir:</span><span class="sxs-lookup"><span data-stu-id="c32d6-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="c32d6-120">Balises et stratégies de rétention</span><span class="sxs-lookup"><span data-stu-id="c32d6-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="c32d6-121">Appliquer une stratégie de rétention aux boîtes aux lettres</span><span class="sxs-lookup"><span data-stu-id="c32d6-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="c32d6-122">Ajouter ou supprimer des balises de rétention</span><span class="sxs-lookup"><span data-stu-id="c32d6-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="c32d6-123">Comment identifier le type de conservation placé sur une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="c32d6-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
