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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468855"
---
<span data-ttu-id="b8b71-p101">Des problèmes d’archivage des éléments à la boîte aux lettres d’Archive. Assurez-vous que vous avez effectué les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="b8b71-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="b8b71-p102">Vérifiez qu’une **Archive de boîte aux lettres** a été activé. Si ce n’est pas le cas, utilisez les étapes de [cet article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) pour activer la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="b8b71-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="b8b71-106">Dans le centre d’administration Exchange, sélectionnez **Les balises de rétention** , sous **Gestion de la conformité**, créez une **balise de rétention** avec l’action **déplacer vers l’Archive** contenant **l’Âge de rétention**votre choix.</span><span class="sxs-lookup"><span data-stu-id="b8b71-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="b8b71-107">Dans le centre d’administration Exchange, sélectionnez les **Stratégies de rétention**, créer une **Stratégie de rétention** et ajouter votre balise de rétention **déplacer vers l’Archive** à cette stratégie.</span><span class="sxs-lookup"><span data-stu-id="b8b71-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="b8b71-p103">[Attribuer la stratégie de rétention](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aux boîtes aux lettres de l’utilisateur. La même stratégie s’appliqueront à **principale** et à la boîte aux lettres **d’Archive** .</span><span class="sxs-lookup"><span data-stu-id="b8b71-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="b8b71-p104">Boîte aux lettres de l’utilisateur doit maintenant avoir une stratégie d’archivage pour déplacer des éléments vers la boîte aux lettres d’Archive. Il peut être nécessaire de forcer la gérées dossier Compagnon (MFA) pour exécuter et appliquer les nouveaux paramètres de boîte aux lettres de l’utilisateur. Exécutez la commande suivante lors [connecté à PowerShell EXO](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) pour démarrer l’Assistant dossier géré pour une boîte aux lettres spécifique :</span><span class="sxs-lookup"><span data-stu-id="b8b71-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="b8b71-113">Plus d’informations sur la configuration d’une stratégie d’archivage, voir [configurer une stratégie d’archivage et de suppression des boîtes aux lettres](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b8b71-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

