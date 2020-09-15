---
title: 'Erreur : les règles de cet ordinateur ne correspondent pas.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690961"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="39c9a-102">Erreur : les règles de cet ordinateur ne correspondent pas.</span><span class="sxs-lookup"><span data-stu-id="39c9a-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="39c9a-103">Pour afficher l’État mis à jour de ce problème connu, consultez [les règles de cet ordinateur ne correspondent pas aux règles de Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="39c9a-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="39c9a-104">L’équipe Outlook a implémenté un correctif dans Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="39c9a-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="39c9a-105">Le correctif est déjà Insider rapidement et sera dirigé vers le canal mensuel de la fin du 2020 juin.</span><span class="sxs-lookup"><span data-stu-id="39c9a-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="39c9a-106">Une fois que vous disposez de la version corrigée, vous pouvez obtenir l’invite « quelles règles souhaitez-vous conserver » une dernière fois.</span><span class="sxs-lookup"><span data-stu-id="39c9a-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="39c9a-107">Choisissez serveur lorsque vous y êtes invité, puis revenez dans Outlook et réactivez toutes les règles qui ont été désactivées.</span><span class="sxs-lookup"><span data-stu-id="39c9a-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="39c9a-108">Tant que le correctif n’est pas disponible, utilisez la solution de contournement suivante :</span><span class="sxs-lookup"><span data-stu-id="39c9a-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="39c9a-109">**Solution**: dans les rapports récents, le problème s’est produit pour ceux qui ont uniquement créé des règles de client dans le bureau Outlook.</span><span class="sxs-lookup"><span data-stu-id="39c9a-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="39c9a-110">Si vous continuez à rencontrer le problème, envisagez de supprimer les règles, puis créez et modifiez des règles uniquement dans OWA (Outlook Web App) jusqu’à ce que le problème soit résolu.</span><span class="sxs-lookup"><span data-stu-id="39c9a-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="39c9a-111">Si vous ne pouvez pas supprimer les règles manuellement, vous pouvez exécuter une commande Outlook lorsque vous démarrez Outlook en exécutant Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="39c9a-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="39c9a-112">Cette opération supprimera les règles client et serveur.</span><span class="sxs-lookup"><span data-stu-id="39c9a-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="39c9a-113">Il supprime toutes les règles de tous les comptes dans le profil Outlook.</span><span class="sxs-lookup"><span data-stu-id="39c9a-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="39c9a-114">Cette commande est encore documentée dans l’article des commutateurs de ligne de commande.</span><span class="sxs-lookup"><span data-stu-id="39c9a-114">This command is further documented in the Command-line switches article.</span></span>

