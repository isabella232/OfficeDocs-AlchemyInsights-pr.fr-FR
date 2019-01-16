---
title: Comment faire pour désactiver les groupes externes
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287900"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="eadcb-102">Comment faire pour désactiver les groupes externes</span><span class="sxs-lookup"><span data-stu-id="eadcb-102">How to disable External Groups</span></span>

<span data-ttu-id="eadcb-p101">Yammer de messagerie externe s’applique les règles de Transport Exchange (ETRs), un ensemble de contrôles proactives pour empêcher les informations sur la société d’être partagé. Afin d’empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer pour la règle de Transport Exchange permet de bloquer la messagerie externe.</span><span class="sxs-lookup"><span data-stu-id="eadcb-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="eadcb-105">Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer :</span><span class="sxs-lookup"><span data-stu-id="eadcb-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="eadcb-106">Se connecter à Yammer comme un administrateur vérifié et dans **Centre d’administration de Yammer**, accédez à C **écurité et sécurité \> paramètres de sécurité.**</span><span class="sxs-lookup"><span data-stu-id="eadcb-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="eadcb-107">Sous **Messagerie externe**, sélectionnez **appliquer votre Exchange Online règles de Transport Exchange (ETRs) dans Yammer.**</span><span class="sxs-lookup"><span data-stu-id="eadcb-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="eadcb-108">Sélectionnez **Save (Enregistrer)**.</span><span class="sxs-lookup"><span data-stu-id="eadcb-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="eadcb-109">Pour plus d’informations, consultez [contrôle externe de la messagerie dans un réseau Yammer avec des règles de Transport Exchange](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="eadcb-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

