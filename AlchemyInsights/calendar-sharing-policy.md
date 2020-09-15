---
title: Stratégie de partage de calendrier 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684228"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="9f7f6-102">Erreur de stratégie lors du partage d’un calendrier</span><span class="sxs-lookup"><span data-stu-id="9f7f6-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="9f7f6-103">Effectuez l’une des opérations suivantes, selon votre situation :</span><span class="sxs-lookup"><span data-stu-id="9f7f6-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="9f7f6-104">Connectez-vous à Exchange Online à l’aide de PowerShell à distance.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="9f7f6-105">Pour plus d’informations, consultez la rubrique [connexion à Exchange Online à l’aide de Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9f7f6-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="9f7f6-106">Sur le serveur local, ouvrez l’environnement de commande Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="9f7f6-107">Déterminer la stratégie de partage qui est attribuée à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="9f7f6-108">Pour ce faire, exécutez la commande suivante et notez la stratégie renvoyée :</span><span class="sxs-lookup"><span data-stu-id="9f7f6-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="9f7f6-109">Mettez à jour la stratégie de partage pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="9f7f6-110">Pour cela, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="9f7f6-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="9f7f6-111">Ouvrez le Centre d’administration Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="9f7f6-112">Cliquez sur **organisation**, puis double-cliquez sur la stratégie qui est attribuée à l’utilisateur sous **partage individuel**.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="9f7f6-113">Il s’agit de la stratégie qui a été renvoyée à l’étape 2.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="9f7f6-114">Dans la page règle de partage, sélectionnez le niveau de partage de calendrier que vous souhaitez autoriser sous **Spécifiez les informations que vous souhaitez partager**; Cliquez sur **Enregistrer**.</span><span class="sxs-lookup"><span data-stu-id="9f7f6-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="9f7f6-115">Pour plus d’informations, voir : ["la stratégie n’autorise pas l’octroi d’autorisations à ce niveau à un ou plusieurs destinataires" lorsque l’utilisateur tente de partager le calendrier](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="9f7f6-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
