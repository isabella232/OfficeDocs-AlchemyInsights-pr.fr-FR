---
title: 'Erreur : les règles sur cet ordinateur ne correspondent pas'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782950"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="6118b-102">Erreur : les règles sur cet ordinateur ne correspondent pas</span><span class="sxs-lookup"><span data-stu-id="6118b-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="6118b-103">Pour voir l'état mis à jour de ce problème connu, consultez Les règles de cet ordinateur ne correspondent pas aux règles [sur Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="6118b-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="6118b-104">L'équipe Outlook a implémenté un correctif dans la build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="6118b-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="6118b-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span><span class="sxs-lookup"><span data-stu-id="6118b-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="6118b-106">Une fois que vous avez la build fixe, vous pouvez obtenir l'invite « Quelles règles voulez-vous conserver » une dernière fois.</span><span class="sxs-lookup"><span data-stu-id="6118b-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="6118b-107">Sélectionnez Serveur lorsque vous y êtes invité, puis revenir dans Outlook et réactivez les règles qui ont été désactivées.</span><span class="sxs-lookup"><span data-stu-id="6118b-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="6118b-108">Jusqu'à ce que le correctif soit disponible, utilisez la solution de contournement suivante :</span><span class="sxs-lookup"><span data-stu-id="6118b-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="6118b-109">**Solution de contournement**: dans les rapports récents, le problème s'est produit pour ceux qui ont uniquement créé des règles client dans le bureau Outlook.</span><span class="sxs-lookup"><span data-stu-id="6118b-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="6118b-110">Si vous continuez à vous lancer dans le problème, envisagez de supprimer les règles, puis créez et modifiez des règles uniquement dans OWA (Outlook Web App) jusqu'à ce que le problème soit résolu.</span><span class="sxs-lookup"><span data-stu-id="6118b-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="6118b-111">Si vous ne pouvez pas supprimer les règles manuellement, vous pouvez exécuter une commande Outlook lorsque vous démarrez Outlook en exécutant Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="6118b-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="6118b-112">Cela supprime à la fois les règles client et serveur.</span><span class="sxs-lookup"><span data-stu-id="6118b-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="6118b-113">Il supprime toutes les règles pour tous les comptes du profil Outlook.</span><span class="sxs-lookup"><span data-stu-id="6118b-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="6118b-114">Cette commande est davantage documentée dans l'article Commutateurs de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="6118b-114">This command is further documented in the Command-line switches article.</span></span>

