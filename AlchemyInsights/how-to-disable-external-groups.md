---
title: Désactivation des groupes externes
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384823"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="39dba-102">Désactivation des groupes externes</span><span class="sxs-lookup"><span data-stu-id="39dba-102">How to disable External Groups</span></span>

<span data-ttu-id="39dba-103">La messagerie externe Yammer applique les règles de transport Exchange (ETR), un ensemble de contrôles proactifs pour empêcher le partage des informations de l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="39dba-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="39dba-104">Pour empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer de façon à ce qu’il utilise la règle de transport Exchange pour bloquer la messagerie externe.</span><span class="sxs-lookup"><span data-stu-id="39dba-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="39dba-105">Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer:</span><span class="sxs-lookup"><span data-stu-id="39dba-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="39dba-106">Connectez-vous à yammer en tant qu’administrateur vérifié, puis, dans le **Centre d’administration Yammer**, accédez à C **contenu \> and Security Security Settings.**</span><span class="sxs-lookup"><span data-stu-id="39dba-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="39dba-107">Sous **messagerie externe**, sélectionnez **appliquer vos règles de transport Exchange Online Exchange (ETR) dans Yammer.**</span><span class="sxs-lookup"><span data-stu-id="39dba-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="39dba-108">Choisissez **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="39dba-108">Choose **Save**.</span></span>

<span data-ttu-id="39dba-109">Pour plus d’informations, reportez-vous à [la rubrique contrôler la messagerie externe dans un réseau Yammer avec des règles de transport Exchange](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="39dba-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  