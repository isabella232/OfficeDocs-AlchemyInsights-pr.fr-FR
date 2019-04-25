---
title: Désactivation des groupes externes
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399589"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="3fad4-102">Désactivation des groupes externes</span><span class="sxs-lookup"><span data-stu-id="3fad4-102">How to disable External Groups</span></span>

<span data-ttu-id="3fad4-103">La messagerie externe Yammer applique les règles de transport Exchange (ETR), un ensemble de contrôles proactifs pour empêcher le partage des informations de l'entreprise.</span><span class="sxs-lookup"><span data-stu-id="3fad4-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="3fad4-104">Pour empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer de façon à ce qu'il utilise la règle de transport Exchange pour bloquer la messagerie externe.</span><span class="sxs-lookup"><span data-stu-id="3fad4-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="3fad4-105">Une fois que vous avez créé une règle dans le centre d'administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer:</span><span class="sxs-lookup"><span data-stu-id="3fad4-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="3fad4-106">Connectez-vous à yammer en tant qu'administrateur vérifié et dans le **Centre d'administration Yammer**, accédez à C **ontent \> et paramètres de sécurité de la sécurité.**</span><span class="sxs-lookup"><span data-stu-id="3fad4-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="3fad4-107">Sous **messagerie externe**, sélectionnez **appliquer vos règles de transport Exchange Online Exchange (ETR) dans Yammer.**</span><span class="sxs-lookup"><span data-stu-id="3fad4-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="3fad4-108">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="3fad4-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="3fad4-109">Pour plus d'informations, reportez-vous à [la rubrique contrôler la messagerie externe dans un réseau Yammer avec des règles de transport Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="3fad4-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

