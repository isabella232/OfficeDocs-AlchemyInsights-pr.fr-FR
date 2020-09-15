---
title: Désactivation des groupes externes
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704126"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="99133-102">Désactivation des groupes externes</span><span class="sxs-lookup"><span data-stu-id="99133-102">How to disable External Groups</span></span>

<span data-ttu-id="99133-103">La messagerie externe Yammer applique les règles de transport Exchange (ETR), un ensemble de contrôles proactifs pour empêcher le partage des informations de l’entreprise.</span><span class="sxs-lookup"><span data-stu-id="99133-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="99133-104">Pour empêcher les utilisateurs de créer des groupes externes, vous devez configurer une règle de transport Exchange (ETR), puis configurer Yammer de façon à ce qu’il utilise la règle de transport Exchange pour bloquer la messagerie externe.</span><span class="sxs-lookup"><span data-stu-id="99133-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="99133-105">Une fois que vous avez créé une règle dans le centre d’administration Exchange Online, procédez comme suit pour définir ETR à appliquer dans Yammer :</span><span class="sxs-lookup"><span data-stu-id="99133-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="99133-106">Connectez-vous à yammer en tant qu’administrateur vérifié, puis, dans le **Centre d’administration Yammer**, accédez à C **contenu and Security \> Security Settings.**</span><span class="sxs-lookup"><span data-stu-id="99133-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="99133-107">Sous **messagerie externe**, sélectionnez **appliquer vos règles de transport Exchange Online Exchange (ETR) dans Yammer.**</span><span class="sxs-lookup"><span data-stu-id="99133-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="99133-108">Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="99133-108">Choose **Save**.</span></span>

<span data-ttu-id="99133-109">Pour plus d’informations, consultez [la rubrique désactiver la messagerie externe dans un réseau Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="99133-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  