---
title: Corriger la stratégie de connexion
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568496"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="5e2a7-102">Corriger la stratégie de connexion</span><span class="sxs-lookup"><span data-stu-id="5e2a7-102">Fix connection policy</span></span>

<span data-ttu-id="5e2a7-103">L’e-mail a été marqué comme sécurisé et remis dans la boîte de réception de l’utilisateur, car l’adresse IP d’envoi a été marquée comme étant sûre dans la stratégie de filtrage des connexions.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="5e2a7-104">Pour passer en revue la stratégie, faites les choses suivantes :</span><span class="sxs-lookup"><span data-stu-id="5e2a7-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="5e2a7-105">Go to the [Office 365 Security & Compliance Center,](https://go.microsoft.com/fwlink/p/?linkid=2077143)and then go to **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="5e2a7-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="5e2a7-106">Sous **l’onglet** Personnalisé, sélectionnez la stratégie **de filtrage des** connexions, puis sélectionnez Modifier la **stratégie.**</span><span class="sxs-lookup"><span data-stu-id="5e2a7-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="5e2a7-107">Examinez la **liste d’adresses IP** autoriser.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="5e2a7-108">Voir si **la liste sécurisée** est activée.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5e2a7-109">Microsoft souscrit à des sources tierces d'expéditeurs dignes de confiance.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="5e2a7-110">Si **la liste fiable** est activée, ces expéditeurs fiables ne sont pas marqués par erreur comme courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="5e2a7-111">Je recommande de sélectionner cette option, car elle permet de réduire le nombre de faux positifs (bon courrier classé comme courrier indésirable) que vous recevez.</span><span class="sxs-lookup"><span data-stu-id="5e2a7-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
